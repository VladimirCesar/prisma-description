[На главную](/README.md)
# Описание колонок для Ag-grid (column definition)

    const colDef = {
        SVETA: "ZASUN SJUDA KOD",
        A_TO: "PO ZHOPE POLUCHISH",
    }

    Группа колонок "Сегменты":
    {
        headerName: 'segments',
        pinned: 'left',
        child.suppressMovable=false;
        child.marryChildren = true;
        children: [
            {
                field: 'segment*',
                columnGroupShow: 'open',
                headerName: 'сегмент*',
                width: 70,
                filter: "agTextColumnFilter",
            }
        ]
    }

    Группа колонок "Основная":
    {
        headerName: 'main',
        child.suppressMovable=false;
        child.marryChildren = true;
        pinned: 'left',
        children: [
            {
                field: "item_producer", 
                headerName: "Брэнд", 
                width: 105,
                filterParams: {
                    buttons: ['reset'],
                }
            },
            {
                field: "item_is_service", 
                headerName: "Это услуга", 
                width: 50, 
                hide: true,
                filterParams: {
                    buttons: ['reset'],
                }
            },
            {
                field: "item_code", 
                headerName: "Код", 
                width: 45, 
                filter: "agTextColumnFilter",
                filterParams: {
                    buttons: ['reset'],
                }
            },
            {
                field: "item_name", 
                headerName: "Номенклатура", 
                width: 300, 
                filter: "agTextColumnFilter",
                filterParams: {
                    buttons: ['reset'],
                }
            },
            {
                field: "primecost", 
                headerName: "Себест", 
                width: 70, 
                filter: "agNumberColumnFilter",
                filterParams: {
                    buttons: ['reset'],
                }
            },
            {
                field: "item_sku", 
                headerName: "Aртикул", 
                width: 70, 
                filter: "agTextColumnFilter",
                filterParams: {
                    buttons: ['reset'],
                }
            },
            {
                field: "item_quality", 
                headerName: "Качество", 
                width: 70, 
                filter: "agTextColumnFilter",
                filterParams: {
                    buttons: ['reset'],
                }
            },
            {
                field: 'motivation',
                headerName: 'ФОТ',
                width: 115,
            },
            {
                field: "item_toi_name", 
                headerName: "Вид номенклатуры", 
                width: 0,
                hide: true,
                filter: "agTextColumnFilter",
                filterParams: {
                    buttons: ['reset'],
                }
            },
            {
                field: "item_group_name", 
                headerName: "Группа номенклатуры", 
                hide: true, 
                width: 0, 
                rowGroup: true,
                filterParams: {
                    buttons: ['reset'],
                }
            },
            {
                field: 'corridor, 
                headerName: "Ценовой коридор", 
                hide: true, 
                width: 0, 
                rowGroup: true,
                filterParams: {
                    buttons: ['reset'],
                }
            },
            {
                field: "propG.addreqs_name",
                headerName: "Свойство группировки",
                width: 57,
                filter: "agTextColumnFilter",
                hide: true,
                rowGroup: true,
            }

        ]
    }

    Группа колонок "Информация по видам цен": 
    { 
        headerName: 'prices',
        child.suppressMovable=false;
        child.marryChildren = true;
        children: [
            {
                field: 'opp',
                headerName: 'СОП',
                cfe_type: "price",
                width: 45,
                sortable: true;
                filter: "agNumberColumnFilter",
            }, {
                 field: 'balanceDC',
                headerName: 'Ост. РЦ',
                cfe_type: 'num-right-top',
                width: 35,
                sortable: true;
                filter: "agNumberColumnFilter",
            }, {
                headerName: 'В пути РЦ',
                cfe_type: 'num-right-top',
                field: 'transitDC',
                width: 35,
                sortable: true;
                filter: "agNumberColumnFilter",
            }, {
                field: 'soldTotal',
                headerName: 'Прод. Всего',
                cfe_type: 'num-right-top',
                width: 35,
                sortable: true;
                filter: "agNumberColumnFilter",
            }, {
                field: 'shopTotal',
                headerName: 'Ост ТП',
                width: 35,
                sortable: true;
                filter: "agNumberColumnFilter",
            }, {
                field: 'transitTotal',
                headerName: 'В пути ТП',
                width: 35,
                sortable: true;
                filter: "agNumberColumnFilter",
            }, {
                 field: 'margin',
                cfe_type: 'num-right-top',
                headerName: 'Маржа',
                width: 35,
                sortable: true;
                filter: "agNumberColumnFilter",
            }, {
                field: 'marginPercent',
                cfe_type: 'num-right-top',
                headerName: '%',
                width: 35,
                sortable: true;
                filter: "agNumberColumnFilter",
            }, {
                 field: 'pola',
                cfe_type: 'num-right-top',
                headerName: 'ЦПЗ',
                width: 35,
                sortable: true;
            }, {
                headerName: 'Прайс Пост.',
                field: 'suppliersPrice',
                filter: "agNumberColumnFilter",
                width: 35,
                sortable: true;
            }, {
                headerName: 'ДППср'
                field: 'dla'
                width: 45;
                sortable: true;
            }, {
                headerName: "ЧП";
                field: "netProfit";
                width: 57;
                sortable: true;
            }
        ]
    }
    Группа колонок "Информация по складам":
    { 
        headerName: 'Инф. по складам',
        child.suppressMovable=false;
        child.marryChildren = true;
        children: [
            {
                headerName: shop.warehouse_name,
                columnGroupShow: 'open',
                child.suppressMovable=false;
                child.marryChildren = true;
                children: [
                    {
                        field: 'sold.*',
                        columnGroupShow: 'open',
                        headerName: 'Прод.',
                        width: 35,
                        maxWidth: 70,
                        filter: "agNumberColumnFilter",
                    },
                    {
                        field: 'balance.*',
                        columnGroupShow: 'open',
                        headerName: 'Ост.',
                        width: 35,
                        maxWidth: 70,
                        filter: "agNumberColumnFilter",
                    },
                    {
                        field: 'transit.*',
                        columnGroupShow: 'open',
                        headerName: 'В пути',
                        width: 35,
                        maxWidth: 70,
                        filter: "agNumberColumnFilter",
                    },
                    {
                        field: 'dla.*',
                        columnGroupShow: 'open',
                        headerName: 'дпп/дсп',
                        width: 35,
                        maxWidth: 70,
                        filter: "agNumberColumnFilter",
                    },
                ],
            }
        ]
    }