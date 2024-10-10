from flask import Flask, render_template, request, redirect

app = Flask(__name__)

# Home route
@app.route('/')
def home():
    return render_template('index.html')

# Submit route
@app.route('/submit', methods=['POST'])
def submit():
    name = request.form.get('name')
    email = request.form.get('email')
    message = request.form.get('message')
    # Here, you can process the data as needed (e.g., save to a database)
    print(f'Name: {name}, Email: {email}, Message: {message}')
    return redirect('/')

if __name__ == '__main__':
    app.run(host='0.0.0.0', port=5000, debug=True)

