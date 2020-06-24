# wagtail_react_streamfield_demo

Demo site for [wagtail-react-streamfield](https://github.com/wagtail/wagtail-react-streamfield). Bootstrapped with `wagtail start`.

Setup instructions:

```sh
git clone git@github.com:thibaudcolas/wagtail_react_streamfield_demo.git
cd wagtail_react_streamfield_demo
virtualenv -p python3.6 venv
source venv/bin/activate
pip install -r requirements.txt
# Update this with the path to your development build of wagtail-react-streamfield.
pip install -e ../../wagtail/wagtail-react-streamfield
./manage.py migrate
./manage.py createsuperuser
./manage.py runserver
```

Then head to http://127.0.0.1:8000/admin/pages/3/add_subpage/ to create a new BlogPage with StreamField.
