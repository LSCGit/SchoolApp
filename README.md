# SchoolApp
校园App
## 1:登录模块 login
LoginHelp：帮助类  
StartPageFragment：启动页  
GuidePageFragment：引导页  
LoginFragment：登录页  
ForgetPwFragment：忘记密码页
### 1.1 使用
````
//对应的Activity中调用（要求继承AppCompatActivity），且需要创建一个FrameLayout来放置Fragment。
LoginHelp.getInstance().startLogin(R.id.act_login_container,this);
//重写，并在此方法中设置要跳转的Activity
@Override
    public void setSupportProgress(int progress) {
        startActivity(new Intent(this,MainActivity.class));
    }
````

## 2:存储模块 storage

