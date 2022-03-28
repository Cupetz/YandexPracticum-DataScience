# YanexPractucum-DataScience
Здесь собраны мои проекты по курсу Data Science от YandexPracticum. Для просмотра проекта нажмите на его название.

# [1.Проект по предсказанию эффективности золотодобычи](https://nbviewer.org/github/Cupetz/YanexPractucum-DataScience/blob/main/%D0%B8%D1%81%D1%85%D0%BE%D0%B4%D0%BD%D1%8B%D0%B5%20%D1%84%D0%B0%D0%B9%D0%BB%D1%8B%20%D0%BF%D1%80%D0%BE%D0%B5%D0%BA%D1%82%D0%BE%D0%B2/1.%20%D0%9E%D0%B1%D1%83%D1%87%D0%B5%D0%BD%D0%B8%D0%B5%20%D0%BC%D0%BE%D0%B4%D0%B5%D0%BB%D0%B8%20-%20%D0%BF%D1%80%D0%B5%D0%B4%D1%81%D0%BA%D0%B0%D0%B7%D0%B0%D0%BD%D0%B8%D0%B5%20%D1%8D%D1%84%D1%84%D0%B5%D0%BA%D1%82%D0%B8%D0%B2%D0%BD%D0%BE%D1%81%D1%82%D0%B8%20%D0%B7%D0%BE%D0%BB%D0%BE%D1%82%D0%BE%D0%B4%D0%BE%D0%B1%D1%8B%D1%87%D0%B8.ipynb)
- в данном проекте обработана большая база сырых данных о золотодобывающих установках с пропусками, аномальными значениями, большим набором признаков (порядка 80), а так же большой объём технической документации для изучения, чтобы разобраться в ньюансах процессов золотодобычи
- вычленены нужные обучающие и целевые признаки для каждой из двух моделей, проведена предобработка данных и обучены обе требуемые модели
- для обучения моделей о оценки их эффективности была задействована кросс-валидация, применено создание собственной метрики качества через make_score, для подбора оптмальных гиперпараметров задействован метод GridSearch. Для сравнения и поиска наиболее эффективной модели были обучены сразу две - случайного леса и логистической регрессии 
# [2.Проект по определению рисков в нефтедобывающей отрасли](https://nbviewer.org/github/Cupetz/YanexPractucum-DataScience/blob/main/%D0%B8%D1%81%D1%85%D0%BE%D0%B4%D0%BD%D1%8B%D0%B5%20%D1%84%D0%B0%D0%B9%D0%BB%D1%8B%20%D0%BF%D1%80%D0%BE%D0%B5%D0%BA%D1%82%D0%BE%D0%B2/2.%20%D0%9E%D0%B1%D1%83%D1%87%D0%B5%D0%BD%D0%B8%D0%B5%20%D0%BC%D0%BE%D0%B4%D0%B5%D0%BB%D0%B8%20-%20%D0%B2%D1%8B%D0%B1%D0%BE%D1%80%20%D0%BD%D0%B0%D0%B8%D0%BB%D1%83%D1%87%D1%88%D0%B5%D0%B3%D0%BE%20%D1%80%D0%B5%D0%B3%D0%B8%D0%BE%D0%BD%D0%B0%20%D0%B4%D0%BB%D1%8F%20%D0%B4%D0%BE%D0%B1%D1%8B%D1%87%D0%B8%20%D0%BD%D0%B5%D1%84%D1%82%D0%B8.ipynb)
- в данном проекте нужно было оценить риски при выборе определённого реально существующего региона для организации в нём деятельности по добыче нефти - были даны базы данных 3-х регионов с информацией о кол-ве скважин и их характеристиках (объём залежей нефти в каждой из скважин, цена за баррель нефти), а так же была описана экономика самой компании: за сколько они продают нефть и в каких объёмах, каковы их затраты на развёртывание нефтедобывающих установок в новом регионе, сколько нефтедобывающих установок в 1 регионе они могут разместить и т.п.
- данные были предобработаны и изучены, обучена модель для предсказания самых выгодных для нефтедобывающей деятельности скважин в каждом из регионов, вычислена реальная прибыль на каждой из возможных выборок, оценены риски в каждом из регионов уйти в минус, а так же предсказана потенциальная средняя прибыль в каждом из регионов
- оценка рисков проводилась при помощи метода Booststrap , так же как о ценка возможной средней прибыли. После данной оценки был выбран один регион с самым оптмальным соотношением между рисками и потенциальной прибылью
- # [3.Анализ перспективных платформ игрового рынка]  
