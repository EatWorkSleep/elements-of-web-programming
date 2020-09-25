0) Install/Use Python3

1) Create VirtualEnv
   A VirtualEnv (Virtual Environment) is a secluded location for Python to install
   dependencies needed by an application.
   You should create separate VirtualEnv for every application.

   python3.8 -m venv venv

2) Activate VirtualEnv

   . venv/bin/activate

3) Install Python libraries and dependencies

   pip install -r requirements.txt

4) Run Programs:   

   a) hello.py

     Open two terminals.

     Terminal 1 (this is the terminal in which you activated your virtual environment):
     ------------

     export FLASK_APP=hello.py

     python -m flask run

     Terminal 2:
     ------------
     - curl http://127.0.0.1:5000/
     - curl http://127.0.0.1:5000/web-programming
     - curl http://127.0.0.1:5000/web-programming/
     - curl "http://127.0.0.1:5000/queryparam?param1=abc&param2=def"
     - curl "http://127.0.0.1:5000/queryparam?param1=abc&param2=def&param3=ghi"
     - curl "http://127.0.0.1:5000/queryparam?param1=abc"
     - curl -v http://127.0.0.1:5000/ut/courses -X POST -H "Content-Type: application/json" -d@course.json
     - curl -v http://127.0.0.1:5000/ut/courses -X POST -H "Content-Type: application/json" -d@course1.json
     - curl -v http://127.0.0.1:5000/ut/courses -X POST -H "Content-Type: application/json" -d@course2.json
     - curl http://127.0.0.1:5000/ut/courses/1 | python -m json.tool
     - curl http://127.0.0.1:5000/ut/courses/2 | python -m json.tool
     - curl http://127.0.0.1:5000/ut/courses/3 | python -m json.tool
     
   b) xmlparse.py

      python xmlparse.py






