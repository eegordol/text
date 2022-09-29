В далёком 2012 году довелось мне участвовать в одном интересном проекте - BuyinUsa. Идея проекта была в следующем: объединить в одном месте товарные предложения с наиболее популярных торговых площадок США, представить их российским потребителям, взять на себя доставку и конвертацию при оплате.

Для начала решили взять самые крупные: ebay, amazon, zappos. К тому же в этот год zappos вообще закрыл возможность для российских пользователей даже заходить на их сайт. А тут мы такие…

Как, наверно, кто-то еще помнить, тогда вездесущего алиэкспресс еще не было, да и умением покупать за границей отличались лишь “продвинутые интернетчики”, а наша задача была предложить услугу как можно более массовому потребителю.

Я выступал в роли и соучредителя и в качестве, как бы сейчас сказали, тимлида, так как вся разработка проекта была на мне. Я был еще достаточно юным и пылал энтузиазмом:)

Вся разработка осуществлялась удаленно, программисты, вебмастер, дизайнер и я работали исключительно через сеть. Использовались в основном простые средства вроде teamview и skype. В качестве основы для сайта взяли всем известную Joomla, а для интернет-магазина Virtualmart. Конечно, по современным воззрениям это ужас-ужас, но тогда мне так не казалось.

Что надо было решить:

1. Карточка товаров, которые были очень разноплановые. А от характеристик зависела возможность отфильтровать товары в поиске.

Решение: взяли более ста карточек с разными характеристиками и просили их отсортировать по важности знакомых и друзей. Сравнивали результаты и выделяли главные. А потом скопировали карточку с Запоса и отредактировали её под свои нужды:)

2. Объединение товаров с таких разных площадок.

У каждой площадки был свой APi, которые мог отдавать данные. Пришлось у всех зарегится как разработчикам, получить ключи и так далее. Сложности были в скорости отдачи, нам же нужна была страница с результатами поиска от каждой площадки и их объединение на нашей странице с сортировкой по цене, размеру, цвету и так далее.
А для запоса пришлось еще прокси в Германии использовать, так как в Россию он не давал данные.

3. Перерасчёт стоимости с долларов на рубли и прибавление комиссии нашей.

Самое простое:) Брали курс с ЦБ, прибавляли 10% и выдавали.

4. Расчёт стоимости доставки в Россию. Очень сложно. Дело в том, что если у Амазона через APi почти всегда передавался вес и геометрические размеры, то у Ebay это было далеко не для каждого товара. Поэтому пришлось часть товаров показывать без стоимости доставки, а её рассчитывать уже при оформлении заказа.

5. Дизайн. Сложности были в том, что каждый имел своё мнение об этом, но мне удалось в итоге предложить компромиссный вариант.

Скажу честно, сейчас бы я не взялся за такой проект, так как просто не представлял всех сложностей для его реализации. Но тогда … Работал не отлипая от компа, с перерывами на сон с ноября 2011 по март 2012. И в результате у нас стало получаться.

Скорость загрузки страниц была очень высокой, во всяком случае задержка с получением данных с площадок была почти незаметна, сортировка выдавала нужные позиции и цены получались вполне привлекательные.
Оставалось дело за рекламой…

Итак, мы уже имели вполне работоспособный сайт, который взаимодействовал через api с тремя площадками в сша: ebay, amazon и zappos. Когда пользователь на нашем сайте делал поисковый запрос, например, iphone, он передавался на площадки и уже оттуда приходили результаты поиска, которые отражались у нас. Похожим образом были устроены и каталоги, при клике например на обувь, запрос шел на площадки и полученные результаты отображались у нас. Уже с ценой в рублях с нашей комиссией и возможностью добавить эти товары в корзину. Другими словами, в онлайне всё было готово для работы, за исключением онлайн оплаты. Здесь были сложности, в основном не технические, а юридические.

Также нужен был склад для пересылки товаров, которые нельзя было сразу отправить из США в России, так как продавец не делал такую услугу. Один из учредителей как раз и обладал опытом работы в Америке и должен был это организовывать.

Для решения задачи была зарегистрирована фирма в США, она же арендовала склад в безналоговом штате (имеется в виду отсутствие налога с продаж), куда должны были поступать покупки. Сервис, конечно, в США был хорош. Просто установили программу для печати посылочных бланков, в ней сразу происходила оплата и распечатывание уже оплаченного бланка. После этого посылку просто можно было забросить в ближайшую почту USPS. В дальнейшем планировалось оправка посылок через какой-нибудь сервис, чтобы зарабатывать и на доставке.

Рекламу разместили в Директе, я использовал динамические объявления с динамическими же ссылками. Virtualmart с нашим напиллингом:) позволил получать для каждого товара уникальные ссылки, заканчивающиеся названием продукта.

Что-то вроде www.buyinusa.co/xxxxx?.../nike-air-max.xml Поэтому по запросу в поисковике nike купить сразу появлялось рекламное объявление с этой ключевой фразой и ведущее на страницу такого товара.

Сложности были в настройке бюджета, потому что некоторые запросы были очень дорогие, а конверсий почти не давали. Тем не менее, стали появляться заказы, которые надо было обрабатывать и выполнять. И здесь увы мы не справились.

Проблему усугубилось тем, что как раз в этот год Почта России столкнулась с большим увеличением посылок из-за границы и там настал коллапс. Уверен, кто нибудь помнит жуткие очереди на Проспекте Вернадского, где отделение ЕМС находится.

В общем, чуток был раньше… или позже, вполне возможно, проект бы смог вырасти.

Разработка обошлась примерно в 30 тысяч баксов, в основном это зарплата программистов, вебмастера, дизайн, аренда сервера и другие подобные расходы. Была также поездка в США и некоторые расходы на разработку схемы движения финансов.

Что в результате? Опыт, знания, злоба и хороший багаж знаний по этой теме.

Сайт достаточно долго работал потом без поддержки и еще долго приходили заказы. Которые не выполнялись. Как не смешно, но немного заработать удалось на референтных ссылках, можно было прямо из карточки товара, который с Амазон, перейти на него. И таких переходов, закончившихся там покупками, было не так уж мало.

Скриншотов сайта не осталось, нашел только некоторые рисунки. Вот такой был хедер и визитка.
