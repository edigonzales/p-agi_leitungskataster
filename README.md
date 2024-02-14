# p-agi_leitungskataster

```
docker compose -f ../gretljobs/docker-compose.yml run --rm -u $UID --workdir //home/gradle/schema-jobs/shared/schema \
  gretl -PtopicName=agi_lkmap -PschemaDirName=schema createSchema configureSchema
```

java -jar /Users/stefan/apps/ili2pg-4.11.1/ili2pg-4.11.1.jar --dbhost localhost --dbport 54321 --dbdatabase edit --dbusr ddluser --dbpwd ddluser --dbschema agi_lkmap_v1 --models "SIA405_LKMap_2015_LV95" --disableValidation --defaultSrsCode 2056 --dataset 2546_was --import data/2546_was.xtf
