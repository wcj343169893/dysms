# dysms
Aliyun SMS SDK for CakePHP 3.0+

1. 复制DySmsComponent到\src\Controller\Component
2. https://ak-console.aliyun.com/ 从这里找到ACCESS_ID和ACCESS_KEY ，如果没有，生成一个
3. PagesController控制器中，引入DySms模块
> var $components = [
>    'DySms'
>];
4. 调用发送方法
>public function index(){
>    $this->DySms->send();
>}
