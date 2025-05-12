## FigureGeneration
# FA_figuregeneration


# Обязательная часть 
# 1 пункт
Реализовать API, которое позволяет генерировать, преобразовывать и визуализировать последовательность плоских полигонов, представленных в виде картежа картежей (например: ((0,0), (0,1), (1,1), (1,0)) — представление для квадрата). Последовательности представлений полигонов представляют собой итераторы (далее: последовательности полигонов). Решать задачи с использованием функционального стиля программирования, в том числе активно использовать функции из модуля itertools и functools.


<img width="582" alt="image" src="https://github.com/user-attachments/assets/dd3f893d-cd1c-44aa-bd0f-daa703a70343" />



<img width="1099" alt="image" src="https://github.com/user-attachments/assets/bf8a98eb-3c4c-4954-a62b-4db8d24b01f0" />




# 2 пункт
Реализовать функции, генерирующие бесконечную последовательность непересекающихся полигонов с различающимися координатами (например, «ленту», см. рис. 2):
прямоугольников (gen_rectangle);



<img width="577" alt="image" src="https://github.com/user-attachments/assets/fff1e0f6-6143-416d-ad04-16fe3faa5d42" />



треугольников (gen_triangle);

<img width="876" alt="image" src="https://github.com/user-attachments/assets/e5384b61-ef86-4070-813c-21450f3bc1da" />






<img width="625" alt="image" src="https://github.com/user-attachments/assets/f4622f41-8681-415a-9bda-5d29c4468625" />


правильных шестиугольников (gen_hexagon).


<img width="883" alt="image" src="https://github.com/user-attachments/assets/24604619-46a3-4e92-8706-498a7d855dcd" />




<img width="1136" alt="image" src="https://github.com/user-attachments/assets/9ee370a2-6627-4523-936f-8889c3ecc15a" />



с помощью данных функций используя функции из модуля itertools сгенерировать семь фигур, включающих как прямоугольники, так и треугольники и шестиугольники, визуализировать результат.



# 3 пункт


Реализовать операции:


параллельный перенос
 (tr_translate);

 <img width="598" alt="image" src="https://github.com/user-attachments/assets/a91553ae-4c00-4734-b078-ec84b2b884a0" />


 <img width="560" alt="image" src="https://github.com/user-attachments/assets/bea7b7b4-7289-4081-ad94-f77fa285f401" />



поворот (tr_rotate);


<img width="872" alt="image" src="https://github.com/user-attachments/assets/5a22ef98-2bb6-4015-9297-066c7fb4cf01" />



<img width="611" alt="image" src="https://github.com/user-attachments/assets/e6e25e26-13bf-4489-9f8e-31bdc46e62e0" />


симметрия (tr_symmetry);

<img width="601" alt="image" src="https://github.com/user-attachments/assets/3179f43a-add5-4a9f-b373-720921093dcc" />


<img width="755" alt="image" src="https://github.com/user-attachments/assets/c2b185e3-632b-4d2c-b5ef-00cefd5753b7" />



гомотетия (tr_homothety);

<img width="809" alt="image" src="https://github.com/user-attachments/assets/57f26783-0604-4520-99e5-26c7ff5e8116" />


<img width="605" alt="image" src="https://github.com/user-attachments/assets/18a3bd03-ddae-4ff3-89e4-db27cf281f7e" />

которые можно применить к последовательности полигонов с помощью функции map.





# 4 пункт

С помощью данных функций создать и визуализировать (рис. 3):
три параллельных «ленты» из последовательностей полигонов, расположенных под острым углом к оси абсцисс;

<img width="714" alt="image" src="https://github.com/user-attachments/assets/25bb8f6a-40ac-433a-b186-d4dbfb4ae8b8" />

<img width="587" alt="image" src="https://github.com/user-attachments/assets/f133fa83-aea7-4efe-b59a-58955121c3e0" />


две пересекающихся «ленты» из последовательностей полигонов, пересекающихся не в начале координат;

<img width="621" alt="image" src="https://github.com/user-attachments/assets/5530ca8b-a3e0-40f6-8d2d-ce3ba8c1c31f" />


<img width="569" alt="image" src="https://github.com/user-attachments/assets/1c0295f0-dd2b-4732-ba2a-705d0aae665b" />


две параллельных ленты треугольников, ориентированных симметрично друг к другу;

<img width="590" alt="image" src="https://github.com/user-attachments/assets/50ffec9f-31c9-4308-9f9d-51f611fa0127" />

<img width="711" alt="image" src="https://github.com/user-attachments/assets/f2d8d4a3-ebdd-46ae-b14d-d6e9954c6e2f" />


последовательность четырехугольников в разном масштабе, ограниченных двумя прямыми, пересекающимися в начале координат.

<img width="822" alt="image" src="https://github.com/user-attachments/assets/0faa226c-9527-4240-9ff0-fb60b3bb0bee" />


<img width="620" alt="image" src="https://github.com/user-attachments/assets/e9bd62e7-1d79-4475-9fa6-5d82d3a7925e" />





# 5 пункт
фильтрации фигур, являющихся выпуклыми многоугольниками (flt_convex_polygon);

<img width="630" alt="image" src="https://github.com/user-attachments/assets/08ba9fff-37a3-4ae8-b756-7c3ae66f1030" />


<img width="505" alt="image" src="https://github.com/user-attachments/assets/5d82de27-eff4-47ce-bbf1-a6450765dd38" />

фильтрации фигур, имеющих хотя бы один угол, совпадающий с заданной точкой (flt_angle_point);
при угле (0,0)

<img width="600" alt="image" src="https://github.com/user-attachments/assets/54f201b1-ecaa-455e-abea-e15435e5535e" />



фильтрации фигур, имеющих площадь меньше заданной (flt_square);

<img width="603" alt="image" src="https://github.com/user-attachments/assets/e4d74c0e-0988-42eb-8788-b1bb94424a7b" />









# 6 пункт
С помощью данных функций реализовать и визуализировать:
фильтрацию фигур, созданных в рамках пункта 4.4; подобрать параметры так, чтобы на выходе было получено шесть фигур;
<img width="806" alt="image" src="https://github.com/user-attachments/assets/20b0a0c2-6a22-4d64-b82f-0d32e5c8e028" />







# 7 пункт 

Реализовать декораторы и продемонстрировать корректность их работы:

преобразующие многоугольники в итераторах среди аргументов функции, работающие на основе функций из п. 3:


@tr_translate,

<img width="864" alt="image" src="https://github.com/user-attachments/assets/fda2aeb1-d3ed-4f37-9da6-a15228b92757" />
@tr_rotate, 

<img width="632" alt="image" src="https://github.com/user-attachments/assets/bceb8b1a-5c81-451b-8777-c18eae04efd6" />

@tr_symmetry, 

<img width="726" alt="image" src="https://github.com/user-attachments/assets/afb3c5aa-cbfe-4b35-b131-8b338cd798cd" />


@tr_homothety.


<img width="702" alt="image" src="https://github.com/user-attachments/assets/b12ef01b-1dbd-436f-857a-1864b1a67c55" />



# 8 пункт 

Реализовать функции и продемонстрировать их корректность

поиск самого длинной стороны многоугольника (agr_max_side);
<img width="756" alt="image" src="https://github.com/user-attachments/assets/32fcd316-070e-48da-8d14-eea8ab964cae" />


поиск самой маленькой площади многоугольника (agr_min_area);

<img width="629" alt="image" src="https://github.com/user-attachments/assets/2f9850e0-a830-4eaf-88ef-25ca5db68a9e" />


расчет суммарного периметра (agr_perimeter);
<img width="754" alt="image" src="https://github.com/user-attachments/assets/03c8f60f-3134-409b-a025-c5bddd4b9257" />





