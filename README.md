# Deploying a basic ML app in Google Cloud Run built using Streamlit

## Building container image
```bash
gcloud builds submit --tag gcr.io/clean-monitor-330012/streamlit-testapp  --project=clean-monitor-330012
```

## Deploying to Google Cloud Run
```bash
gcloud run deploy --image gcr.io/clean-monitor-330012/streamlit-testapp --platform managed  --project=clean-monitor-330012 --allow-unauthenticated
```

### Output Public URL
![Output Public URL](https://raw.githubusercontent.com/shamanthMuroor/cloudRepo/main/screenshots/output%20-%20public%20url.png)


### Service Account Permissions Enabled
![Service Account Permissions Enabled](https://raw.githubusercontent.com/shamanthMuroor/cloudRepo/main/screenshots/service%20account%20permissions.png)


### Build History
![Build History](https://raw.githubusercontent.com/shamanthMuroor/cloudRepo/main/screenshots/build%20history.png)


### Container Images
![Container Images](https://raw.githubusercontent.com/shamanthMuroor/cloudRepo/main/screenshots/container%20images.png)


### Cloud Run After Deploying
![Cloud Run After Deploying](https://raw.githubusercontent.com/shamanthMuroor/cloudRepo/main/screenshots/cloud%20run%20deployed.png)


### App Metrics
![App Metrics](https://raw.githubusercontent.com/shamanthMuroor/cloudRepo/main/screenshots/app%20metrics.png)


### To Allow or Disallow Public Access
1. Select Project -> Right side permissions tab, delete Cloud Run Invoker/Choose Add Principal
![Allow or Disallow public access](https://raw.githubusercontent.com/shamanthMuroor/cloudRepo/main/screenshots/Allowing%20or%20Disabling%20public%20access.png)

2. To add permission: Select Role:*Cloud Run Invoker*  to Principal:*allUsers*
![Adding permission for public access](https://raw.githubusercontent.com/shamanthMuroor/cloudRepo/main/screenshots/Cloud%20run%20invoker-allUsers%20for%20public%20access.png)


### Pricing of Cloud Resource Used
1. Cloud Run Pricing
![Cloud Run Pricing](https://raw.githubusercontent.com/shamanthMuroor/cloudRepo/main/screenshots/Cloud%20Run%20Pricing.png)

2. Cloud Storage Pricing
![Cloud Storage Pricing](https://raw.githubusercontent.com/shamanthMuroor/cloudRepo/main/screenshots/Cloud%20Storage%20Pricing%20for%20Buckets.png)
