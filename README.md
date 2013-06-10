top
===

淘宝API接口简易封装 Python

使用前你需要做什么
=================

该库实现使用了[requests](https://pypi.python.org/pypi/requests)库，如果需要使用urllilb2等实现请求，请自行实现
需要配置taobao.py应用参数

使用范例
=======


    from top import TopRequest

    req = TopRequest()
    req['fields'] = 'seller_nick,buyer_nick,title,type,created,tid,seller_rate,buyer_rate,\
                     status,payment,adjust_fee,post_fee,total_fee,pay_time,end_time,\
                     modified,consign_time,buyer_obtain_point_fee,real_point_fee,\
                     received_payment,commission_fee,pic_path,num_iid,num,price,cod_fee,\
                     cod_status,shipping_type,receiver_name,receiver_state,receiver_city,\
                     receiver_district,receiver_address,receiver_zip,receiver_mobile,\
                     receiver_phone,orders.tid,orders.title,orders.pic_path,orders.price,\
                     orders.num,orders.sku_id,orders.refund_status,orders.status,orders.oid,\
                     orders.total_fee,orders.payment,orders.discount_fee,orders.adjust_fee,\
                     orders.sku_properties_name,orders.item_meal_name,orders.buyer_rate,\
                     orders.seller_rate,orders.outer_iid,orders.outer_sku_id,\
                     orders.refund_id,orders.seller_type'

    client = TopClient()
    response = client.execute(
        req, session="62007306f38614dbf4a11b3d56f1ccff87c350ZZ96d0782670923820")


更多例子
=====

参考淘宝API接口和[top.py](https://github.com/thomashuang/top/blob/master/top.py)

