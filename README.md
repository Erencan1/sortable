# sortable
Make HTML table interactive and sortable
Check out table.js, it is easily customizable


```javascript

    var example_sortingFunction = function (row) {
        var total = parseInt(row.cells[2].innerHTML) + parseInt(row.cells[3].innerHTML)
        var minutes = parseInt(row.cells[4].innerHTML)
        return -total/minutes;
    };

    stage({
        'table_id': 'exp_table_id', // HTMLTableElement id,
        'row_counter': 6, // row number to display on one page,
        'sortingFunction': example_sortingFunction, // leave null, if sorting is not needed when page is loaded
    });
    
```
