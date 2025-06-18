# Prerequisites
* install boto3
* log into an aws account

# Get size per first level folder from the given prefix 

## usage 
python3 s3_folder_sizes.py mybucket/optionalprefix

### output sample
```
mybucket/optionalprefix/folder1: 50MB
mybucket/optionalprefix/folder2: 20MB
```


# Get size per second level folder from the given prefix 
python3 s3_folder_sizes_2level.py mybucket/optionalprefix

### output sample
```
mybucket/optionalprefix/folder1/secondlevel1: 20MB
mybucket/optionalprefix/folder1/secondlevel2: 30MB
mybucket/optionalprefix/folder2/secondlevel1: 10MB
mybucket/optionalprefix/folder2/secondlevel2: 7MB
mybucket/optionalprefix/folder2/secondlevel3: 3MB
```
