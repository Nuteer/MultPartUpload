# MultPartUpload
This project can be used to upload files directly to an S3 bucket using S3’s Multipart upload strategy. With this strategy, files are chopped up in parts of 5MB+ each, so they can be uploaded concurrently. It’s also quite reliable: if a single part fails to upload, only that 5MB chunk has to be retried.
