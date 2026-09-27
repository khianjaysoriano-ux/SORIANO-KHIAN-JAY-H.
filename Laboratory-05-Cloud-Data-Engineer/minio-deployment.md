
# MinIO Object Storage Server Deployment Documentation

## Deployment Specifications

- **Container Engine:** Docker
- **Image:** `minio/minio`
- **Console Web Port:** `9001`
- **API Port:** `9000`
- **Target Bucket Name:** `client-photos`

## Deployment Command

The MinIO S3-compatible storage server was deployed using the following Docker command:

```bash
docker run -d -p 9000:9000 -p 9001:9001 --name minio-server \
  -e "MINIO_ROOT_USER=cloudadmin" \
  -e "MINIO_ROOT_PASSWORD=CloudNova2026!" \
  minio/minio server /data --console-address ":9001"
