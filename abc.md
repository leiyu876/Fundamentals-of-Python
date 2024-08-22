Here are 10 different variants of Python code for writing a file:

**Variant 1: Simple Write**
```
with open('example.txt', 'w') as f:
    f.write('Hello, World!')
```
**Variant 2: Write with Mode**
```
with open('example.txt', 'w+', encoding='utf-8') as f:
    f.write('Hello, World!')
```
**Variant 3: Write with Buffering**
```
with open('example.txt', 'w', buffering=1024) as f:
    f.write('Hello, World!')
```
**Variant 4: Write with Encoding**
```
with open('example.txt', 'w', encoding='latin-1') as f:
    f.write('Hello, World!')
```
**Variant 5: Write with Newline**
```
with open('example.txt', 'w', newline='\n') as f:
    f.write('Hello, World!')
```
**Variant 6: Write with Append Mode**
```
with open('example.txt', 'a') as f:
    f.write('Hello, World!')
```
**Variant 7: Write with Binary Mode**
```
with open('example.bin', 'wb') as f:
    f.write(b'Hello, World!')
```
**Variant 8: Write with Text Mode and Encoding**
```
with open('example.txt', 'wt', encoding='utf-16') as f:
    f.write('Hello, World!')
```
**Variant 9: Write with Comma Separated Values (CSV)**
```
import csv
with open('example.csv', 'w', newline='') as f:
    writer = csv.writer(f)
    writer.writerow(['Hello', 'World'])
```
**Variant 10: Write with JSON**
```
import json
with open('example.json', 'w') as f:
    json.dump({'message': 'Hello, World!'}, f)
```
Note that these variants demonstrate different ways to write to a file, including:

* Simple write
* Writing with specific modes (e.g. `w+`, `a`, `wb`)
* Writing with buffering
* Writing with specific encodings (e.g. `utf-8`, `latin-1`)
* Writing with newline characters
* Writing in binary mode
* Writing in text mode with encoding
* Writing comma-separated values (CSV)
* Writing JSON data
Here are 10 different variants of Python code for appending to a file:

**Variant 1: Simple Append**
```
with open('example.txt', 'a') as f:
    f.write('Hello, World!')
```
**Variant 2: Append with Encoding**
```
with open('example.txt', 'a', encoding='utf-8') as f:
    f.write('Hello, World!')
```
**Variant 3: Append with Newline**
```
with open('example.txt', 'a', newline='\n') as f:
    f.write('Hello, World!')
```
**Variant 4: Append to a Binary File**
```
with open('example.bin', 'ab') as f:
    f.write(b'Hello, World!')
```
**Variant 5: Append with Buffering**
```
with open('example.txt', 'a', buffering=1024) as f:
    f.write('Hello, World!')
```
**Variant 6: Append to a Text File with Encoding**
```
with open('example.txt', 'at', encoding='utf-16') as f:
    f.write('Hello, World!')
```
**Variant 7: Append Multiple Lines**
```
with open('example.txt', 'a') as f:
    f.write('Hello, World!\n')
    f.write('This is another line.\n')
```
**Variant 8: Append with a Loop**
```
with open('example.txt', 'a') as f:
    for i in range(5):
        f.write(f'Line {i+1}\n')
```
**Variant 9: Append to a CSV File**
```
import csv
with open('example.csv', 'a', newline='') as f:
    writer = csv.writer(f)
    writer.writerow(['Hello', 'World'])
```
**Variant 10: Append to a JSON File**
```
import json
with open('example.json', 'a') as f:
    json.dump({'message': 'Hello, World!'}, f)
    f.write('\n')
```
Note that these variants demonstrate different ways to append to a file, including:

* Simple append
* Appending with specific encodings (e.g. `utf-8`, `utf-16`)
* Appending with newline characters
* Appending to a binary file
* Appending with buffering
* Appending to a text file with encoding
* Appending multiple lines
* Appending with a loop
* Appending to a CSV file
* Appending to a JSON file
Here are 10 different variants of Python code for reading a JSON file:

**Variant 1: Simple Read**
```
import json
with open('example.json') as f:
    data = json.load(f)
print(data)
```
**Variant 2: Read with Encoding**
```
import json
with open('example.json', encoding='utf-8') as f:
    data = json.load(f)
print(data)
```
**Variant 3: Read with Buffering**
```
import json
with open('example.json', buffering=1024) as f:
    data = json.load(f)
print(data)
```
**Variant 4: Read a JSON Array**
```
import json
with open('example.json') as f:
    data = json.load(f)
    for item in data:
        print(item)
```
**Variant 5: Read a JSON Object**
```
import json
with open('example.json') as f:
    data = json.load(f)
    print(data['key'])
```
**Variant 6: Read a Nested JSON Object**
```
import json
with open('example.json') as f:
    data = json.load(f)
    print(data['key']['nested_key'])
```
**Variant 7: Read a JSON File with Comments**
```
import json
import re
with open('example.json') as f:
    content = f.read()
    content = re.sub(r'//.*', '', content)
    data = json.loads(content)
print(data)
```
**Variant 8: Read a Large JSON File**
```
import json
with open('example.json') as f:
    data = []
    for line in f:
        data.append(json.loads(line))
print(data)
```
**Variant 9: Read a JSON File with Error Handling**
```
import json
try:
    with open('example.json') as f:
        data = json.load(f)
    print(data)
except json.JSONDecodeError as e:
    print(f"Error parsing JSON: {e}")
```
**Variant 10: Read a JSON File using `json.JSONDecoder`**
```
import json
decoder = json.JSONDecoder()
with open('example.json') as f:
    data = decoder.decode(f.read())
print(data)
```
Note that these variants demonstrate different ways to read a JSON file, including:

* Simple read
* Reading with specific encodings (e.g. `utf-8`)
* Reading with buffering
* Reading a JSON array
* Reading a JSON object
* Reading a nested JSON object
* Reading a JSON file with comments
* Reading a large JSON file
* Reading a JSON file with error handling
* Reading a JSON file using `json.JSONDecoder`
