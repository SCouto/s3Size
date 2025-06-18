# Prerequisites
* install boto3
* log into an aws account

# Get size per first level folder from the given prefix 

## usage 
python3 s3_folder_sizes.py mybucket/optionalprefix

### output sample
```
mybucket/optionalprefix/folder1: 50 MB
mybucket/optionalprefix/folder2: 20 MB
```


# Get size per second level folder from the given prefix 

## usage 
python3 s3_folder_sizes_2level.py mybucket/optionalprefix

### output sample
```
mybucket/optionalprefix/folder1/secondlevel1: 20 MB
mybucket/optionalprefix/folder1/secondlevel2: 30 MB
mybucket/optionalprefix/folder2/secondlevel1: 10 MB
mybucket/optionalprefix/folder2/secondlevel2: 7 MB
mybucket/optionalprefix/folder2/secondlevel3: 3 MB
```

## usage  with an output file
python3 s3_folder_sizes_2level.py mybucket/optionalprefix --output=myFile.csv

### output sample
```
mybucket/optionalprefix/folder1/secondlevel1;20 MB
mybucket/optionalprefix/folder1/secondlevel2;30 MB
mybucket/optionalprefix/folder2/secondlevel1;10 MB
mybucket/optionalprefix/folder2/secondlevel2:;7 MB
mybucket/optionalprefix/folder2/secondlevel3;3 MB
```


