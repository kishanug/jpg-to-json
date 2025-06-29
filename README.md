import csv
import json
csv_file=('file_path')
json_file='otput_path'
with open(csv_file,mode='r',encoding='utf-8') as f:
    reader=csv.DictReader(f)
    data=list(reader)

with open(json_file, mode='w', encoding='utf-8') as f:
    json.dump(data, f, indent=4)
