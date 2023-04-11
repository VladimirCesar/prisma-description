
# Параметры, используемые для формировании таблицы

<table style="overflow-x: scroll;" border="1">
    <thead>
        <tr>
            <th>Наименование</th>
            <th>Поле</th>
            <th>Тип</th>
            <th>Примечание</th>
        </tr>
    </thead>
    <tbody>
        <tr>
            <td>Период</td>
            <td>settings.periods</td>
            <td>Object[{name: String, value: Number}]</td>
            <td>Массив объектов, содержащих наименование периода и его значение</td>
        </tr>
        <tr>
            <td>Дата начала отчета</td>
            <td>settings.dateStart</td>
            <td>Date</td>
            <td>Дата, дата (без времени)</td>
        </tr>
        <tr>
            <td>Дата окончания отчета</td>
            <td>settings.dateEnd</td>
            <td>Date</td>
            <td>Дата, дата (без времени)</td>
        </tr>
        <tr>
            <td>Рабочая дата</td>
            <td>settings.workDate</td>
            <td>Date</td>
            <td>Дата, дата (без времени)</td>
        </tr>
        <tr>
            <td>Сегменты</td>
            <td>settings.segments</td>
            <td>String[]</td>
            <td>Массив GUID'ов, ссылок на группы сегментов</td>
        </tr>
        <tr>
            <td>Виды цен</td>
            <td>settings.typeOfPrices</td>
            <td>String[]</td>
            <td>Массив GUID'ов, ссылок на виды цен</td>
        </tr>
        <tr>
            <td>Склады</td>
            <td>settings.warehouses</td>
            <td>String[]</td>
            <td>Массив GUID'ов, ссылок на склады</td>
        </tr>
        <tr>
            <td>Виды номенклатуры</td>
            <td>settings.typeOfItems</td>
            <td>String[]</td>
            <td>Массив GUID'ов, ссылок на виды номенклатуры</td>
        </tr>
        <tr>
            <td>Постраничный скроллинг</td>
            <td>settings.paging</td>
            <td>Boolean</td>
            <td>Флаг, включен ли постраничный скроллинг</td>
        </tr>
    </tbody>
</table>
<image src="/res/settings_screen.png" alt="Настройки ПРИЗМА">