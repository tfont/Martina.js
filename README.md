# Martina.js
Create readable JavaScript in PHP

    create a change on #date

    if the value on this instance is not empty
        fetch the url of http://localhost/_lola/fnr/school-search/api/getDay.php
            and set its method to post
            and set its headers as
                accept: application/json
                content-type: application/json
            and set its body to use
                JSON object stringify with 
                    date: the value on this instance
        after fetch
        then 
        then
        and finally catch an exception
        
    ending the change on #date


Or alternately directly through PHP.

```php
$data = 'http://localhost/api/getDay.php';
$make = new MartinaJS;


$javascript = $make->process(function () use ($data)
{
    return text::javascript()
    ->m('create a change on #date')
    ->m('')    
        ->m('if the value on this instance is not empty')    
        ->m('fetch the url of '.$data)    
            ->m('and set its method to post')    
            ->m('and set its headers as')    
                ->m('accept: application/json')    
                ->m('content-type: application/json')    
            ->m('and set its body to use')    
                ->m('JSON object stringify with')    
                    ->m('date: the value on this instance')    
       ->m('after fetch')    
       ->m('then)    
       ->m('then')    
       ->m('and finally catch an exception')    
    ->m('')    
    ->m('ending the change on #date')    
});

echo $javascript;
```

By, Travis van der Font
