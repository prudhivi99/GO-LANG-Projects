# Use an official Go runtime as a parent image
FROM golang:1.17-alpine3.15

# Set the working directory in the container
WORKDIR /app

# Copy the local package files to the container's workspace
COPY . .

# Initialize modules (optional, but good practice)
RUN go mod init hello-docker

# Build the Go executable
RUN go build -o hello .

# Run the hello binary when the container starts
CMD ["./hello"]
