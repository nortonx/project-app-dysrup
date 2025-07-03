# Use an official PostgreSQL image as the base image
FROM postgres:14.11-alpine

# Update system packages to reduce vulnerabilities
RUN apk update && apk upgrade --no-cache

# Set the working directory inside the container
WORKDIR /app

# Set environment variables for the PostgreSQL database
ENV POSTGRES_USER=postgres
ENV POSTGRES_PASSWORD=postgres
ENV POSTGRES_DB=nest_finance_tracker

# Expose the PostgreSQL port
EXPOSE 5432

# Define the command to start the PostgreSQL server
CMD ["postgres"]
