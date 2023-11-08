# pathology-server-setup
This repo has all the tools required to setup the environment for pathology images processing and storing


> Start the minio and easypanel
```
docker-compose -f docker-compose.yml up --build --force-recreate
```

> Libvips usage
```
vips dzsave $INPUT $OUTPUT --vips-concurrency=30 --vips-progress --suffix=".webp" --strip --tile-size=1024 --compression=4 
```
> Minio default username and passoword
>> minioadmin:minioadmin

> Minio default urls

>> S3-API: http://172.21.0.3:9000  http://127.0.0.1:9000


>> Console: http://172.21.0.3:9090 http://127.0.0.1:9090 

> Easypanel default urls
>> http://127.0.0.1:3000

docker-compose -f docker-compose.yml up --build --force-recreate