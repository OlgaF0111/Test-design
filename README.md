### Задача 1. Система скорринга рассчитывает % ставку по кредиту для клиента исходя из его возраста, который вводится в форму:  
От 18 до 25 лет – 18%  
От 25 до 45 лет – 16 %  
Свыше 45 лет – 20% 

Демонстрируется применение техник: эквивалентного разбиения, граничных значений.

Решение:  
____
1. Применение техники эквивалентного разбиения:
   
Возраст 75 лет определен на основании статистических данных взятых из Интернета (максимальный возраст кредитования в банках России), т.к. не представлена исчерпывающая информация в условиях задачи.  

| Диапазон |число в диапазоне (пример)|% ставка по кредиту| 
| ---------| ------------------------ |------------------ | 
|[18; 25]  |15                        |0%                 |  
|[18; 25]  |22                        |18%                |
|[25; 45]  |30                        |16%                |
|[45; 75]  |51                        |20%                |
|[45; 75]  |84                        |0%                 |

2. Применение техники граничных значений
   
| Диапазон |число в диапазоне (пример)|% ставка по кредиту| 
| ---------| ------------------------ |------------------ | 
|[18; 25]  |17;                       |0%                 |  
|[18; 25]  |18; 19; 24; 25;           |18%                |
|[18; 25]  |26;                       |16%                |
|[25; 45]  |44; 45;                   |16%                |
|[25; 45]  |46;                       |20%                |
|[45; 75]  |74; 75;                   |20%                |
|[45; 75]  |76;                       |0%                 |

### Задача 2.  Проверка поля Фамилия, какие проверку могут быть в рамках эквивалентного разбиения. 

Решение:  
___
1.	Минимальное и максимальное количество букв в поле  
2.	Латиница, кириллица  
3.	Спецсимволы, цифры  
4.	Верхний и нижний регистр  
5.	Первая буква в фамилии пишется с большой буквы  
6.	Двойная фамилия через дефис, через пробел  
7.	Буква Ё в фамилии  
8.	Обязательность заполнения поля

### Задача 3. Есть интернет-магазин, который предлагает:  		  					
- Скидку постоянного покупателя от 5% до 20%.	  		  														
- Количество вещей, которые курьер привезет бесплатно от 1 до 6. Это такие плюшки за лояльность и повторную покупку.  

Как плюшки высчитываются? Есть два условия:      		  															
- Сколько клиент потратил — бонус добавляется при достижении 100р, 500, 1000 и 5000 руб    																	
- Какой % выкупа — бонус получаем при достижении 5%, 30%, 50% и 80%.
                     				
Если клиент потратил 100р и почти ничего не выкупил — скидки не дадут и вещей мало привезут.
Если потратил больше и выкупил больше, то дадут небольшую скидку. И так далее.      	

Скидка и количество бесплатных вещей исходя из % выкупа в Таблицах 1 и 2.  
Таблица 1.        							 
|% выкупа| потрачено| скидка пп в %| кол-во вещей | 							
| ------ | -------- | ------------ | ------------ | 							
|5%      | 100      |  0           | 1            |  							
|5%      | 500      |  5           | 1            |							
|5%      | 1 000    |  10          | 2            |							
|5%      | 5 000    |  15          | 3            |							
|30%     | 100      |  0           | 2            |  							
|30%     | 500      |  5           | 3            |							
|30%     | 1 000    |  10          | 4            |							
|30%     | 5 000    |  15          | 5            |							
|50%     | 100      |  5           | 2            |  							
|50%     | 500      |  10          | 3            |							
|50%     | 1 000    |  15          | 4            |							
|50%     | 5 000    |  20          | 5            |							
|80%     | 100      |  5           | 3            |  							
|80%     | 500      |  10          | 4            |							
|80%     | 1 000    |  15          | 5            |							
|80%     | 5 000    |  20          | 6            |

Таблица 2.  
|% выкупа| потрачено| скидка пп в %| кол-во вещей | 							
| ------ | -------- | ------------ | ------------ | 							
|5%      | 5 100    |  15          | 4            |  							
|5%      | 5 500    |  15          | 4            |							
|5%      | 6 000    |  15          | 4            |							
|5%      | 6 500    |  15          | 4            |							
|30%     | 5 100    |  15          | 5            |  							
|30%     | 5 500    |  15          | 5            |							
|30%     | 6 000    |  15          | 5            |							
|30%     | 6 500    |  15          | 5            |							
|50%     | 5 100    |  20          | 5            |  							
|50%     | 5 500    |  20          | 5            |							
|50%     | 6 000    |  20          | 5            |							
|50%     | 6 500    |  20          | 5            |							
|80%     | 5 100    |  20          | 6            |  							
|80%     | 5 500    |  20          | 6            |							
|80%     | 6 000    |  10          | 6            |							
|80%     | 6 500    |  20          | 6            |

Демонстрируется применение техники "Таблица принятия решений".  

Решение:  
___
Таблица 1.1. ![image](https://github.com/OlgaF0111/Test-design-/assets/123538617/03f9e747-0b99-4e68-a24e-206bca23f0ae)  
Таблица 2.2. ![image](https://github.com/OlgaF0111/Test-design-/assets/123538617/adc389e7-e980-43e0-b7c0-7c6242daccaf)  
В диапазоне покупок от 100 до 5000 руб, тестирую все ТС (тестовые сценарии) представленные в Таблице 1.1, т.к. количество доставляемых вещей и % скидки разные и зависят от суммы покупки и % выкупа. В диапазоне покупок от 5100 до 6500 руб, возьму по одному ТС (это - ТС 17 с 5 % выкупа, ТС 22 с 30% выкупа, ТС 27 с 50% выкупа, ТС 32 с 80% выкупа), т.к. количество вещей доставляемых бесплатно и % скидки одинаково для каждого % выкупа.  

### Задача 4. Стоимость доставки посылки: 
* до 10 кг-130руб  
* до 25 кг-285руб   
* до 50 кг-410руб  
* до 75 кг-536руб   
* до 100 кг-544руб   
* от 100 кг-832руб.
        
Демонстрируется применение техники граничных значений.  

Решение:   
____

| диапазон         |граничные значения      | стоимость доставки|  							
| ---------------- | ---------------------- | ----------------- | 					
|0 кг              |0                       | 0.000 руб         |  					
|от 0.001 до 10кг  |0.001; 9.999; 10.000;   | 130руб            |  						
|от 10.001 до 25кг | 10.001; 24.999; 25.000;|285руб		   	 |	
|от 25.001 до 50кг | 25.001; 49.999; 50.000;|410руб			  	 |	
|от 50.001 до 75кг | 50.001; 74.999; 75.000;|536руб 				 |
|от 75.001 до 100кг| 75.001; 99.999; 100.000;|544руб				 |
|от 100.001        | 100.001;               |832руб 				 |
  							
 


