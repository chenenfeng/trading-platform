activate virtual environment:  source venv/bin/activate
run django server(localhost:8000): python3 manage.py runserver

app

url designate in project -> include app url -> import app views -> request and return template html

navbar: bootstrap.com   documentation

## When you write html, strictly hold the format: {% endif %}. Do not make mistakes on space like { % endif % }


        {% for key, value in api.items %}
            {{ key }}: {{ value }}<br/>
        {% endfor %}

{% if ticker %}
    {{ ticker }}
{% endif %}

else:
        return render(request, 'home.html', {'ticker': "Enter a Ticker Symbol Above"})
    
failed to push some refs to 'git@github.com:chenenfeng/trading-platform.git':
reason: no Readme file in local project

solution:
git stash 
git pull –rebase 
git stash pop
git pull --rebase origin master

change code:
git add .
git commit -am "add code"
git push
