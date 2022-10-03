# Fake OpenRTB DSP Server

## OpenRTB 2.6 & OpenRTB Native Ads Specification 1.2

### Фейковая DSP(Demand Side Platform) для валидации OpenRTB BidRequest запросов форматов Native, Banner, Video, Audio с отдачей валидных OpenRTB BidResponse ответов. 



### Основные особенности и возможности.


* Валидируются только объекты и значения BidRequest указаные как required в спецификации. 

* Полная поддержка спецификации OpenRTB 2.6 & OpenRTB Native Ads Specification 1.2, включая множетственные объекты Imp в одном BidRequest запросе, а так же соместный запрос Native, Banner, Video, Audio объектов в одном объекте Imp ( п. 3.2.4 Спецификации OpenRTB 2.6 ). 

* На каждый объект Native, Banner, Video, Audio объектов в одном объекте Imp фейковая DSP отвечает BidResponse объектом с  необхдимым количеством Bid объектов с указанием impid & mtype в соответствии с спецификацией.

* В ответе BidResponse поддерживается множество SeatBid объектов с множеством Bid объектов, в соответствии с спецификацией.