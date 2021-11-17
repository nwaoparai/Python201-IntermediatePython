from collections import ChainMap<br/><br/>

car_parts = {'hood': 500, 'engine': 5000, 'front_door': 750}<br/>
car_options = {'A/C': 1000, 'Turbo': 2500, 'rollbar': 300}<br/>
car_accessories = {'cover': 100, 'hood_ornament': 150, 'seat_cover': 99}<br/>
car_pricing = ChainMap(car_accessories, car_options, car_parts)<br/>
print(car_pricing['hood'])
