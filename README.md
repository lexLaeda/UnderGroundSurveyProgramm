# UndergroundSurveyProgramm
                                    
                                                                         Профильное описание
   Данная программа производит расчет основных параметров съемочной точки(средняя часть программы) в тоннеле(радиус,смещение, пикетаж, отклонение по высоте),
 расчет производится от двух заданных точек оси тоннеля(в левой части программы). 
 Точки можно забить вручную, или можно импортировать из форматированного текстового файла), можно использовать файл съемки из электронного тахеометра, предварительно его отредактировав в текстовом редакторе.
 Также после расчета основных параметров точек, можно получить относительные отклонения всей плоскости объекта, которому принадлежат съемочные точки) и при монтаже нового кольца тоннеля учесть данные отклонения)
 Учитывая что в электронных тахеометрах, используемых в ОАО "Метрострой" отсутсвует функция расчета отклонений от плоскости, программу можно использовать для этого, забив две координаты вектора перпендикулярного
 плоскости съемки(первая точка должна принадлежать съемочной плоскости).
 
                                                                        Математическое описание
   Если абстрагироваться от задач тоннелестроения, то в левую часть программы забиваются координаты(X,Y,H) 2 точек(Пк первой точки можно принять равной нулю, 
 второй может иметь любое положительное значение). В центральной части программы забиваются координаты любых других точек или тех же самых. При выполнении расчета, программа вычисляет расстояние между первой точкой прямой и
 проекции точки на заданную прямую в пространстве, расстояние между первой точкой и проекцией точки на прямую на плоскости, длину перпендикуляра от точки к прямой в пространстве, длину перпендикуляра от точки к прямой на плоскости
 и превышение точки относительно точки пересечения перпендикуляра от точки к прямой. Второй расчет сравнивает все полученные расстояния от проекции точки до первой точки прямой с минимальным и расчитывает относительные значения.
 
 test