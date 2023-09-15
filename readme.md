# Installation
### Global
```shell script
sudo curl -L "https://raw.githubusercontent.com/jhmaverick/dns-helper/master/dns-helper" -o /usr/local/bin/dns-helper
sudo chmod +x /usr/local/bin/dns-helper
```

Ex: `dns-helper <cmd>`


### Local
```shell script
curl -L "https://raw.githubusercontent.com/jhmaverick/dns-helper/master/dns-helper" -o ./dns-helper
chmod +x ./dns-helper
```

Ex: `./dns-helper <cmd>` or `bash dns-helper <cmd>`


# Commands
### Display help
```bash
dns-helper --help
```

### Display the nameserver of a domain
```bash
dns-helper nameserver example.com
```

### Display a specific record of a domain
```bash
dns-helper record example.com A
```

### Display records commonly used by domains
```bash
dns-helper records example.com --cpanel-records
```

### Display common records of a domain using a specific resolver
```bash
dns-helper --resolver=1.1.1.1 records example.com
```

### Show records commonly used by domains in zone file format
```bash
dns-helper zone-file example.com > ./example.com.txt
```

### Update the script
```bash
dns-helper update
```

### Display version
```bash
dns-helper version
```
