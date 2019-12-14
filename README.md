nacos作为注册中心时，服务消费端例子

启动
nohup>nohupGps java -jar nacos-consumer.jar 2>&1 &

linux模拟请求测试
curl "http://127.0.0.1:18081/notFound-feign"
curl "http://127.0.0.1:18081/divide-feign?a=5&b=2"
curl "http://127.0.0.1:18081/echo-feign/testnacos"
curl "http://127.0.0.1:18081/services/nacos-provider"
curl "http://127.0.0.1:18081/services"