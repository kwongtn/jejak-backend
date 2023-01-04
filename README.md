Useful commands:

```sh
docker build --tag=kwongtn/rosak_backend:latest --tag=kwongtn/rosak_backend:$(date +%Y%m%d-%H%M) . && docker push kwongtn/rosak_backend:latest
docker exec lift-rosak-backend_db_1 pg_dumpall -U postgres > backup2.sql
cp /mnt/c/Users/tungn/OldDrive/@temp/backup2.sql .
scp -v -i C:\Users\tungn\.ssh\azure-default.pem azureuser@65.52.187.210:/home/azureuser/lift-rosak-backend/backup2.sql C:\Users\tungn\OldDrive\@temp\
psql -U postgres  -f backup2.sql
```

admins = [
"tungnan5636@gmail.com",
"kzy13695@gmail.com",
"vincentkzy22@gmail.com",
"shiraz.nunis8@gmail.com",
"cameronkang91@gmail.com",
"adihusaini80@gmail.com",
"szehoong@gmail.com",
]
