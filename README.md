This project is only for POC purpose.


1 , Python Application.


Pre recruitment,

install python3 and pip , docker 20 , aws account , ECR repo.


 2, How can I build this application ?
 
I have used Flask-Marshmallow for this project is a thin integration layer for Flask (a Python web framework)and marshmallow (an object serialization/deserialization library) that adds additional features to marshmallow, including URL and Hyperlinks fields for HATEOAS-ready APIs. It also (optionally) integrates with Flask-SQLAlchemy.


3, WHy I have used SQLAlchemy ?

SQLAlchemy is the Python SQL toolkit and Object Relational Mapper that gives application developers the full power and flexibility of SQL.

4, Application have 4 part

1, one for getting health check 
2, initializing connection between app and database
3, updating data to Database
4, and getting all data from database
  two get motheod and one post


5, API list 
1, http://domainname:8000/health
2,http://domainname:8000/get
3, http://domainname:8000/post


6, POST method we should use body data as a below  input with json formate


{

	"country": "india",
	"population": "101"
	
}


7, Its contain two files 1, new.py  and Dockerfile is containe all files related this application , it containe a Dockerfile , using this file can build and using aws command can tag and upload image to ECR


