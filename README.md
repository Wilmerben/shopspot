# Shop Spot
An online store for the local shops near you

Shop Spot lists the local bussiness owners near you and lists their services and products. You can either buy them online if they support delivery or you can view the sales prices and choose the best shop.

Setting up Shop Spot is very easy.
## Want to Use?
This branch is under development right now. It is in early stages so there is no specific release for you to use. 
## Building

It is best to use the python `virtualenv` tool to build locally:

```bash
> virtualenv venv
> source venv/bin/activate
> git clone https://github.com/oriefy/shopspot .
```
Then you navigate to the base directory of the project and install the requirements in your virtual environment

```bash
> cd shopspot
> pip install -Ur requirements/local.txt
```
And finally you make migrations to the database, create a super user, and run the server
```bash
> python manage.py makemigrations
> python manage.py migrate
> python manage.py loaddata accounts/fixtures/initial.json
> python manage.py runserver
```

Then visit `http://localhost:8000` to view the app.
Visit `http://localhost:8000/admin` to login to admin with
username: admin@oriefy.com
password: oriefy123

```bash
> foreman start
```
## Hall of fame
Everyone who contributes to ShopSpot gets a spot here.
* [@ZeroCoolHacker](https://github.com/ZeroCoolHacker)
