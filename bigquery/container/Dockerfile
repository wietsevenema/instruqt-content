# base instruqt client image
FROM gcr.io/instruqt-shadow/base

# Authorize gcloud for the Instruqt Shadow project
ADD svc.json svc.json
RUN gcloud auth activate-service-account --key-file=svc.json && rm svc.json

# Install uuidgen
RUN apt-get install uuid-runtime