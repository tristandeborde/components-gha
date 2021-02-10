# Extend the official Rasa image
ARG rasa_version=2.1.2
FROM rasa/rasa:$rasa_version

# Copy components folder to working directory
COPY ./components /app/components

# By best practices, don't run the code with root user
USER 1001

ENV PYTHONPATH "${PYTHONPATH}:/app"