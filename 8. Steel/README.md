# Металлургический комбинат
Есть металлургический комбинат ООО «Так закаляем сталь», который решил оптимизировать расходы на одном из технологических процессов его производства.
________

**Описание данных:** Данные состоят из файлов, полученных из разных источников:

* **data_arc_new.csv** — данные об электродах;
* **data_bulk_new.csv** — данные о подаче сыпучих материалов (объём);
* **data_bulk_time_new.csv** — данные о подаче сыпучих материалов (время);
* **data_gas_new.csv** — данные о продувке сплава газом;
* **data_temp_new.csv** — результаты измерения температуры;
* **data_wire_new.csv** — данные о проволочных материалах (объём);
* **data_wire_time_new.csv** — данные о проволочных материалах (время).

Во всех файлах столбец key содержит номер партии. В файлах может быть несколько строк с одинаковым значением key: они соответствуют разным итерациям обработки.
________

**Задача:** Построить модель, которая предскажет температуру стали.
________

**Цель:** С помощью построенной модели машинного обучения компания должна уменьшить потребление электроэнергии на этапе обработки стали.
________