## Внешний источник данных цл_ПризмаВнешний

Внешний источник данных, база MS SQL «PrismaExternal», протокол обмена TCP/IP.

### Таблицы и их поля :

(жирным шрифтом выделены ключи связи)

---

<h3><u>items - Номенклатура</u></h3>
<table border=1>
    <tr>
        <th>Имя поля</th>
        <th>Тип</th>
        <th>NULLABLE</th>
        <th>Прим.</th>
    </tr>
    <tr>
        <td><strong>id</strong></td>
        <td><strong>str (36)</strong></td>
        <td>-</td>
        <td>GUID</td>
    </tr>
    <tr>
        <td>name</td>
        <td>str (100)</td>
        <td>-</td>
        <td>Рабочее наименование</td>
    </tr>
    <tr>
        <td>sku</td>
        <td>str (50)</td>
        <td>+</td>
        <td>Артикул</td>
    </tr>
    <tr>
        <td>code</td>
        <td>str (11)</td>
        <td>-</td>
        <td>Код</td>
    </tr>
    <tr>
        <td>quality</td>
        <td>str (0)</td>
        <td>+</td>
        <td>Качество</td>
    </tr>
    <tr>
        <td>producer</td>
        <td>str (150)</td>
        <td>+</td>
        <td>Производитель</td>
    </tr>
    <tr>
        <td><strong>type_of_item_id</strong></td>
        <td><strong>str (36)</strong></td>
        <td>-</td>
        <td>GUID вида номенклатуры</td>
    </tr>
    <tr>
        <td><strong>group_id</strong></td>
        <td><strong>str (36)</strong></td>
        <td>-</td>
        <td>GUID родителя</td>
    </tr>
    <tr>
        <td>is_group</td>
        <td>bool</td>
        <td>-</td>
        <td>Признак "Это группа"</td>
    </tr>
</table border=1>

<h3><u>type_of_items - Виды номенклатуры</u></h3>
<table border=1>
    <tr>
        <th>Имя поля</th>
        <th>Тип</th>
        <th>NULLABLE</th>
        <th>Прим.</th>
    </tr>
    <tr>
        <td><strong>id</strong></td>
        <td><strong>str (36)</strong></td>
        <td>-</td>
        <td>GUID</td>
    </tr>
    <tr>
        <td>name</td>
        <td>str (50)</td>
        <td>-</td>
        <td>Наименование</td>
    </tr>
    <tr>
        <td><strong>group_id</strong></td>
        <td><strong>str (36)</strong></td>
        <td>-</td>
        <td>GUID родителя</td>
    </tr>
    <tr>
        <td>is_group</td>
        <td>bool</td>
        <td>-</td>
        <td>Признак "Это группа"</td>
    </tr>
</table border=1>

<h3><u>segments - Сегменты</u></h3>
<table border=1>
    <tr>
        <th>Имя поля</th>
        <th>Тип</th>
        <th>NULLABLE</th>
        <th>Прим.</th>
    </tr>
    <tr>
        <td><strong>id</strong></td>
        <td><strong>str (36)</strong></td>
        <td>-</td>
        <td>GUID</td>
    </tr>
    <tr>
        <td>name</td>
        <td>str (50)</td>
        <td>-</td>
        <td>Наименование</td>
    </tr>
    <tr>
        <td><strong>group_id</strong></td>
        <td><strong>str (36)</strong></td>
        <td>-</td>
        <td>GUID родителя</td>
    </tr>
    <tr>
        <td>is_group</td>
        <td>bool</td>
        <td>-</td>
        <td>Признак "Это группа"</td>
    </tr>
</table border=1>

<h3><u>type_of_prices - Виды цен</u></h3>
<table border=1>
    <tr>
        <th>Имя поля</th>
        <th>Тип</th>
        <th>NULLABLE</th>
        <th>Прим.</th>
    </tr>
    <tr>
        <td><strong>id</strong></td>
        <td><strong>str (36)</strong></td>
        <td>-</td>
        <td>GUID</td>
    </tr>
    <tr>
        <td>name</td>
        <td>str (50)</td>
        <td>-</td>
        <td>Наименование</td>
    </tr>
    <tr>
        <td><strong>group_id</strong></td>
        <td><strong>str (36)</strong></td>
        <td>-</td>
        <td>GUID родителя</td>
    </tr>
    <tr>
        <td>is_group</td>
        <td>bool</td>
        <td>-</td>
        <td>Признак "Это группа"</td>
    </tr>
</table border=1>

<h3><u>warehouses - Склады</u></h3>
<table border=1>
    <tr>
        <th>Имя поля</th>
        <th>Тип</th>
        <th>NULLABLE</th>
        <th>Прим.</th>
    </tr>
    <tr>
        <td><strong>id</strong></td>
        <td><strong>str (36)</strong></td>
        <td>-</td>
        <td>GUID</td>
    </tr>
    <tr>
        <td>name</td>
        <td>str (50)</td>
        <td>-</td>
        <td>Наименование</td>
    </tr>
    <tr>
        <td><strong>group_id</strong></td>
        <td><strong>str (36)</strong></td>
        <td>-</td>
        <td>GUID родителя</td>
    </tr>
    <tr>
        <td>is_group</td>
        <td>bool</td>
        <td>-</td>
        <td>Признак "Это группа"</td>
    </tr>
</table border=1>

<h3><u>period_selects - Периоды формирования отчета</u></h3>
<table border=1>
    <tr>
        <th>Имя поля</th>
        <th>Тип</th>
        <th>NULLABLE</th>
        <th>Прим.</th>
    </tr>
    <tr>
        <td>name</td>
        <td>str (50)</td>
        <td>-</td>
        <td>Наименование</td>
    </tr>
    <tr>
        <td>days</td>
        <td>int (15)</td>
        <td>-</td>
        <td>Количество дней</td>
    </tr>
</table border=1>

<h3><u>shelfs - Полки</u></h3>
<table border=1>
    <tr>
        <th>Имя поля</th>
        <th>Тип</th>
        <th>NULLABLE</th>
        <th>Прим.</th>
    </tr>
    <tr>
        <td><strong>warehouse_id</strong></td>
        <td><strong>str (36)</strong></td>
        <td>-</td>
        <td>GUID склада</td>
    </tr>
    <tr>
        <td><strong>type_of_item_id</strong></td>
        <td><strong>str (36)</strong></td>
        <td>-</td>
        <td>GUID вида номенклатуры</td>
    </tr>
    <tr>
        <td>capacity</td>
        <td>int (15)</td>
        <td>+</td>
        <td>Емкость</td>
    </tr>
    <tr>
        <td>size</td>
        <td>float (15, 2)</td>
        <td>+</td>
        <td>Размер</td>
    </tr>
    <tr>
        <td>additional_capacity</td>
        <td>int (15)</td>
        <td>+</td>
        <td>Емкость подтарки</td>
    </tr>
    <tr>
        <td>comment</td>
        <td>str (100)</td>
        <td>+</td>
        <td>Комментарий</td>
    </tr>
</table border=1>

<h3><u>corridors - Ценовые коридоры</u></h3>
<table border=1>
    <tr>
        <th>Имя поля</th>
        <th>Тип</th>
        <th>NULLABLE</th>
        <th>Прим.</th>
    </tr>
    <tr>
        <td><strong>id</strong></td>
        <td><strong>str (36)</strong></td>
        <td>-</td>
        <td>GUID ценового коридора</td>
    </tr>
    <tr>
        <td>start</td>
        <td>float (15, 2)</td>
        <td>-</td>
        <td>Начало коридора</td>
    </tr>
    <tr>
        <td>end</td>
        <td>float (15, 2)</td>
        <td>-</td>
        <td>Окончание коридора</td>
    </tr>
    <tr>
        <td><strong>type_of_item_id</strong></td>
        <td><strong>str (36)</strong></td>
        <td>-</td>
        <td>GUID вида номенклатуры</td>
    </tr>
</table border=1>

<h3><u>preloaded - Оперативные данные</u></h3>
<table border=1>
    <tr>
        <th>Имя поля</th>
        <th>Тип</th>
        <th>NULLABLE</th>
        <th>Прим.</th>
    </tr>
    <tr>
        <td><strong>item_id</strong></td>
        <td><strong>str (36)</strong></td>
        <td>-</td>
        <td>GUID номенклатуры</td>
    </tr>
    <tr>
        <td><strong>segment_id</strong></td>
        <td><strong>str (36)</strong></td>
        <td>-</td>
        <td>GUID сегмента</td>
    </tr>
    <tr>
        <td><strong>price_id</strong></td>
        <td><strong>str (36)</strong></td>
        <td>-</td>
        <td>GUID вида цены</td>
    </tr>
    <tr>
        <td>price_value</td>
        <td>float (15, 2)</td>
        <td>+</td>
        <td>Цена</td>
    </tr>
    <tr>
        <td><strong>warehouse_id</strong></td>
        <td><strong>str (36)</strong></td>
        <td>-</td>
        <td>GUID склада</td>
    </tr>
    <tr>
        <td>transit_value</td>
        <td>float (15, 3)</td>
        <td>+</td>
        <td>В пути</td>
    </tr>
    <tr>
        <td>balance_value</td>
        <td>float (15, 3)</td>
        <td>+</td>
        <td>Остаток</td>
    </tr>
    <tr>
        <td>auto_motivation_corridor_id</td>
        <td>str (36)</td>
        <td>+</td>
        <td>GUID ценового коридора</td>
    </tr>
    <tr>
        <td>auto_motivation_value</td>
        <td>float (7, 5)</td>
        <td>+</td>
        <td>Автоматическая мотивация</td>
    </tr>
    <tr>
        <td>manual_motivation_sum</td>
        <td>float (15, 2)</td>
        <td>+</td>
        <td>Ручная мотивация, сумма</td>
    </tr>
    <tr>
        <td>manual_motivation_percent</td>
        <td>float (8, 5)</td>
        <td>+</td>
        <td>Ручная мотивация, процент</td>
    </tr>
    <tr>
        <td>sold_value</td>
        <td>float (15, 3)</td>
        <td>+</td>
        <td>Количество продаж</td>
    </tr>
    <tr>
        <td>receipt_days_since_last</td>
        <td>int (4)</td>
        <td>+</td>
        <td>ДПП</td>
    </tr>
    <tr>
        <td>receipt_days_since_old</td>
        <td>int (4)</td>
        <td>+</td>
        <td>ДСП</td>
    </tr>
</table border=1>