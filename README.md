DEDEXT

Be sure that an existing service instance with service name hana and plan type hdi-shared with the name haa-hdi is already in the dev space.

```
mkdir -p target ; mbt build -p=cf -t=target --mtar=haa-cf.mtar ; cf deploy target/haa-cf.mtar -f
```

Substitutions:
```
      "project_name": haahell
      "app_name": myhaa

      "haa_module_name": haa-ina
      "haa_module_dir": haa-java

      "haa_router_name": haa-web
      "haa_router_dir": haa-entry

      "haa_router_name": haa-web
      "haa_router_dir": haa-entry

      "haa_db_name": haa-hdb
      "haa_db_dir": haa-db

      "db_schema_name": 

      "haa_uaa_res_name": haa-uaa
      "haa_uaa_svc_name": haa-uaa
      "haa_hdi_res_name": haa-hdi
      "haa_hdi_svc_name": haa-hdi
      
      "sac_host":  ateam-isveng.us10.sapanalytics.cloud
      "deploy_landscape": us10
      "deploy_dnsdomain": cfapps.us10.hanna.ondemand.com
      "subacct_subdomain": conciletime
      "deploy_space": dev
``` 
# haahell
