# File Handling
 - File handling in Python is one of the many tools that gives it power and versatility, as it can do a lot of operations. However, the same thing should be kept in mind while writing any program in Python: weigh the benefits against the demerits to have a security, reliability, and efficiency-based code.
 
- ** Opening Files:
	
	- *Use open('filename', mode) to open files. Modes include 'r' for reading, 'w' for writing (creates or truncates), 'a' for appending, 'x' for exclusive creation, 'r+' for reading and writing, and 'w+' for writing and reading.

- ** Reading and Writing:

	- *Use file.read() to read the entire file or file.write(data) to write data to the file. Use file.readline() or iterate over file for line-by-line reading.

- ** Resource Management:

	- *Always close files with file.close() after operations. Alternatively, use with open('filename', mode) as file: to automatically close files when done.
	
# CSV Handling
- ** CSV Files:
	Use Python's csv module for reading and writing CSV files. Write rows with csv.writer(file).writerows(data) and read with csv.reader(file).

- ** Serialization and Deserialization
  - *Serialization:

	Convert objects into a format suitable for storage or transmission. Python provides modules like pickle and json.
	Pickle:

	Use pickle.dump(object, file) to serialize objects into a file and pickle.load(file) to deserialize them back into objects. Works with complex Python objects.
	JSON:

	Use json.dumps(data) to serialize Python objects into JSON strings and json.dump(data, file) to write to a file. json.loads(json_string) and json.load(file) deserialize JSON data.
	Example Usage
	- python
	- Copy code
	- Import pickle


# Key Points
- **Persistence: Involves storing and retrieving data across different sessions or systems.
- **File Handling: Essential for reading from and writing to files using various modes.
- **Serialization: Converts objects into a format for storage (e.g., pickle, JSON).
- **Deserialization: Converts serialized data back into usable objects.
- **Best Practices: Always close files properly; use serialization for complex data structures.
