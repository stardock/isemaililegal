# isemaililegal


```  

				/*邮箱检测*/
			if(!validateEmail($email.val())) {
				swal2-show('Oops...', "邮箱不合法,请检查后输入",'error');
					return false;
				}
				/* 邮箱验证 */
				var email_arr = $email.val().split('@');
				var email_blacklist = ["qq.com","sina.com", "163.com","sina.cn", "gmail.com", "live.com", "163.com", "139.com", "outlook.com", "189.cn", "foxmail.com", "vip.qq.com", "hotmail.com", "126.com", "aliyun.com", "yeah.net", "sohu.com", "live.jp", "msn.com", "icloud.com"];
			if ($.inArray(email_arr[1], email_blacklist) == "-1") {
				swal2-show('Oops...', "暂不支持此邮箱，请更换如QQ、谷歌、新浪、网易等常见邮箱。",'error');
				return false;
				}
			function validateEmail(value){
				var pattern = /^\w+([-+.]\w+)*@\w+([-.]\w+)*\.\w+([-.]\w+)*$/;
				if (pattern.test(value)) 
				{
					return true;
				}
				else
				{
					return false;
				}
			}

```  
