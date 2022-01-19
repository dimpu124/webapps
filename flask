from flask import Flask, redirect, url_for, request
app = Flask(__name__)

@app.route('/success/<name>')
def success(name):
    if name == "sona":
        return 'No its Saumya'
    else:
        return 'Yes you are right its Saumya'

@app.route('/login',methods = ['POST', 'GET'])
def login():
   if request.method == 'POST':
      user = request.form['nm']
      return redirect(url_for('success',name = user))
   

if __name__ == '__main__':
   app.run()