# vue-data-table
A simple responsive data table Vue component with no CSS.

Insipred by https://datatables.net/. Who uses jQuery in 2022??

## No CSS
This component uses `<table>` tags and you can style it whatever you like. 
    
## Responsive
Just give an order to your column definition.
- `priority: 0` - column must be always visible.
- `priority: n` – less priority in responsiveness and makes column wrap in case the shortage of width.

## Using
```
<data-table
    :columns="[{
        target: 'id',
        title: 'ID'
    }, {
        target: 'country',
        title: 'Country'
    }, {
        target: 'name',
        title: 'Name'
    }, {
        target: 'phone',
        title: 'Phone number'
    }]"
    :data="[{
        "id": 1,
        "country": "South Korea",
        "name": "Berk Wall",
        "phone": "(115) 677-0123"
    }, {
        "id": 2,
        "country": "Pakistan",
        "name": "Raya Woodward",
        "phone": "(208) 732-5335"
    }, {
        "id": 3,
        "country": "United States",
        "name": "Aileen Estrada",
        "phone": "(551) 731-3118"
    }]">
</data-table>
```
