# GeoData MADE HW

## HW1

- Tast №1. Reading coordinates from a file and creating a geometries
- Task №2. Creating LineStrings that represent the movements
- Task №3. Points to map
- Task №4. Movements of individual user
- Task №5. Join accessibility datasets into a grid and visualize them by using a classifier
- Task №6. Calculate and visualize the dominance areas of shopping centers


## HW2

- Task №1. Hot point:

    Генерируйте рандомные точки на планете Земля до тех пор, пока не попадете на территорию Афганистана.
    1. Вы можете использовать функции принадлжености точки полигону и расстояния от точки до полигона (в метрах)
    2. Предложите не наивный алгоритм поиска (генерировать __напрямую__ точку из полигона границ Афганистана __запрещено__)

- Task №2. Quality of life:

    Для измерения показателя качества жизни в точке, найденной в предыдущем задании, вам необходимо рассчитать следующую сумму расстояний (в метрах):
    1. Расстояние от точки до 5 ближайших __*__ банкоматов, находящихся в стране с наибольшим количеством объектов жилой недвижимости
    2. Расстояние от точки до 5 ближайших школ, находящихся в стране с наибольшим количеством аптек в столице
    3. Расстояние от точки до 5 ближайших кинотеатров, наодящихся в стране с самым большим отношением числа железнодорожных станций к автобусным остановкам в южной     части __**__
    
    __*__ При поиске _N_ ближайших объектов обязательно использовать ``R-tree``

    __**__ Южной частью страны является территория, находящаяся к югу от множества точек, равноудаленных от самой северной и самой южной точек страны
    
- Task №3. NY track:

    Добраться __на автомобиле__ от входа в ``Central Park`` __Нью-Йорка__ (со стороны ``5th Avenue``) до пересечения ``Water Street`` и ``Washington Street`` в         Бруклине (откуда получаются лучшие фото Манхэттенского моста) довольно непросто - разумеется, из-за вечных пробок. Однако еще сложнее это сделать, проезжая мимо     школ, где дети то и дело переходят дорогу в неположенном месте.
    

## HW3

60% of the digital ad inventory is sold by publishers in Real Time first price Auctions.

Once a user lands on a webpage, bidders (advertisers) bid for different ad slots on the page and the one with the highest winning bid displays their ad in the ad space and pays the amount he bid. This process encourages bid shading – bidding lesser than the perceived value of the ad space to maximize utilization for self while maintaining a particular win rate at lowest prices.

Hence, for publishers, it becomes important to value their inventory (all the users that visit their website * all the ad slots they have on their websites) correctly so that a reserve price, or a minimum price can be set up for the auctions.

In a first price auction, the highest bidder wins and pays the price they bid if it exceeds the reserve price. The optimal strategy of a bidder is to shade their bids (bid less than their true value of the inventory). However, bidder needs to win a certain amount to achieve their goals. This suggests they need to shade as much possible while maintaining a certain win rate.

A bidder perceives a certain value out of every impression they win. Each bidder would like to maintain the value they derived out of this set of websites (given in the dataset) in June with a maximum deviation of 20%.

Setting a reserve price induces this by causing bidders to lose at lower bids which encourages higher bidding and more publisher revenue. However, since most of these takes place through automated systems, there might be an unknown delay in setting reserve prices & reducing win rate of bidder & bidder changing their bid shading algorithm & increased publisher revenue.

IMPORTANT TERMS:
- Publisher – person who owns and publishes content on the website
- Inventory – all the users that visit the website * all the ad slots present in the website for the observation period
- Impressions - showing an ad to a user constitutes one impression. If the ad slot is present but an ad is not shown, it falls as “unfilled impression”. Inventory is the sum of impressions + unfilled impressions.
- CPM – cost per Mille. This is one of the most important ways to measure performance. It is. Calculated as revenue/impressions * 1000. 'bids' and 'price' are measured in terms of CPM
