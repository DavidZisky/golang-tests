FROM golang:1.21.1

# Set destination for COPY
WORKDIR /app

# Copy the source code
COPY src/ .

# Download Go modules
RUN go mod download

# Build
RUN go build -o /go-webserver

EXPOSE 3000

# Run
CMD ["/go-webserver"]