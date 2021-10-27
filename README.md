gcloud builds submit --tag gcr.io/clean-monitor-330012/streamlit-testapp  --project=clean-monitor-330012


gcloud run deploy --image gcr.io/clean-monitor-330012/streamlit-testapp --platform managed  --project=clean-monitor-330012 --allow-unauthenticated
