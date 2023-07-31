## filter without worrying about empty arrays

```php
$filterSafeArray = ArraMethods::filter_array([]);
$list = MyDataObject::get()->filter($filterSafeArray);
```

## sort by any id sequence

```php
$sortByStatement = ArraMethods::create_sort_statement_from_id_array([44,222,434,22,]);
$sortedList = MyDataObject::get()->orderBy($sortByStatement);

```
