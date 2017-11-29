# dysms
## Aliyun SMS SDK for CakePHP

1. https://ak-console.aliyun.com/ 从这里找到ACCESS_ID和ACCESS_KEY ，如果没有，生成一个
2. 修改/config/paths.php,最后加入 
> /** 阿里云Access Key ID */
> putenv('OSS_ACCESS_ID=aaa');

> /** 阿里云 ACCESS KEY */
> putenv('OSS_ACCESS_KEY=bbb');
3. PagesController控制器中，引入DySms模块
> var $components = [
>    'DySms.Sms'
>];
4. 调用发送短信方法
>public function index(){
>    $this->Sms->send();
>}
