Chosen Select Widget for Yii 2
=========
- Chosen Select Widget based on Chosen jQuery plugin [chosen](http://harvesthq.github.io/chosen)

Usage
------------
1) Usage with ActiveForm and model
```php
   echo $form->field($model, 'subject')->widget(\softcommerce\chosen\ChosenSelect::className(),[
                    'items' => [
                        'first' => 'First',
                        'second' => 'Second'
                    ],
                ]); 

  ```
  
2) Usage without a model
```php
   echo \softcommerce\chosen\ChosenSelect::widget([
        'name'  => 'select',
        'items' => BooleanEnum::listData(),
        'options' => [
            'width' => '95%'
        ]
    ]);
```

Select Options 
----------------
You can find them on the [options page](http://harvesthq.github.io/chosen/options.html)
