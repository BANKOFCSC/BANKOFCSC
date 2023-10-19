<body>


	<!-- WRAPPER -->
	<div class="form-element">

		<!-- TOP BAR -->
		














<form name="langChangeForm" id="langChangeForm" method="get" action="dashboard?[B@7249a429">
	<input type="hidden" name="lang" id="langFieldId">
</form>



<script>

	function changeAppLanguage(passedLang) {
		var languageStr = "English";
		if (passedLang == "hi_IN") {
			languageStr = "Hindi";
		}

		$('#langPomptMsg')
				.html(
						"Are you sure you want to Change language to "
								+ languageStr
								+ "? <br/> Page will be reloaded! Please Confirm.");
		$('#changeLanguagePromptModel').modal({
			show : true
		});

		$('.promptTrue').unbind("click").click(function(e) {
			//var actionUrl = window.location.pathname;
			var actionUrl = window.location;
			$("#langChangeForm").attr("action",actionUrl);
			$("#langFieldId").val(passedLang);
			$("#langChangeForm").submit();
			//location.href = "dashboard?lang=" + passedLang;
		});

		$('.promptCancel').unbind("click").click(function(e) {
			$('#langPomptMsg').html("");
		});
		return true;
	}
</script>

<!-- Delete Confirmation Custom Prompt Start -->
<div id="changeLanguagePromptModel" class="modal fade confirm" role="dialog">
	<div class="modal-dialog">

		<!-- Modal content-->
		<div class="modal-content oh">
			<div class="modal-header">
				<button type="button" class="close" data-dismiss="modal">×</button>
				<h4 class="modal-title">Language Change Confirmation</h4>
			</div>
			<div class="modal-body">

				<div class="col-sm-12">
					<div class="form-group">
						<span class="col-sm-12 text-center"><strong id="langPomptMsg"></strong></span>
					</div>
					<div class="col-sm-offset-5">
						<span class="btn btn-primary promptTrue"><i class="fa fa-check-circle"></i>OK</span> <span class="btn btn-default promptCancel" data-dismiss="modal">Cancel</span>
					</div>
				</div>
			</div>
			<div class="modal-footer"></div>
		</div>

	</div>
</div>
<!-- Delete Confirmation Custom Prompt End -->
 
<div class="top-bar">
 
	<div class="container">

		<div class="row">
			<div class="col-md-12 ">
				<div class="col-lg-4">
					<a class="navbar-brand" href="#"><img src="resources/assets/images/Ashok_logo.png" alt="logo" class="img-logo"></a>
					<h1 class="logotxt">
						Government of Rajasthan
					</h1>
					<span class="font13">Department of Information Technology &amp; Communication</span>
				</div>
				<div class="col-md-4" style="border: 2px solid rgba(236, 130, 57, 0.71);font-weight: 900;border-radius: 10px 10px 10px 10px;text-align: center;color: #518DC0;margin-top: 10px;">
				
				<div class="col-sm-2"><a href="javascript:void(0)" onclick="$('#open-call-center-app').submit()"><img src="resources/assets/images/reg.gif"></a></div>
				
					
						<div class="col-sm-10" style="font-size:12px;">0141-2922241, 0141-2922238</div>
					
					<div class="col-sm-12"><i class="fa fa-envelope" style="font-size:20px;float:left;padding-left:10px;padding-top:8px"></i>	<div style="font-size:11px;">service.emitra@rajasthan.gov.in helpdesk.emitra@rajasthan.gov.in utility.emitra@rajasthan.gov.in</div></div>
				</div>
				<div class="pull-right ">
					<img src="resources/assets/images/emitra_logo.png">
				</div>
			</div>
		</div>

	<!-- Form to open Call center App Starts-->
	<form id="open-call-center-app" action="http://103.203.138.129/emitracccwp/Login.aspx" method="post" target="_blank">
		<input type="hidden" name="ssoid" id="ssoid" value="MANOJKUMARBALAI813">
		<input type="hidden" name="tokenno" id="tokenno" value="K3BRUXJYRHZNaDBSSmQxQWlaZEVab0FBRFVrOTZRSGx1VE9qVnZPVy9KZ0Z2VXBnWkdqWTBOTjZQSHRMVDAyMDEyQnVRSm9rVkdXV1NCRUd0RjJGa2Vwa0RIa2M2eFlkVkZwN254Y3U1RzJoZnFRVEJxTjFZc2FRelBoUnFER2t1QkRPa1dyOFkveW5Ka1BLZ3owZlNUdE94OVhFbHFURTNDa01ESDU3WXUyRmp5b1Z3NGZLVmVMQ2NpZGFzd2Z3">
		<input type="hidden" name="entitycode" id="entitycode" value="K12290269">
		<input type="hidden" name="role" id="role" value="LSPKIOSK">
		<input type="hidden" name="entityName" id="entityName" value="MANOJ KUMAR BALAI">
		<input type="hidden" name="entityAddress" id="entityAddress" value="BHARAT NIRMAN RAJIV GANDHI SEWA KENDRA">
		<input type="hidden" name="lspnameId" id="lspnameId" value="490">
	</form>
	<!-- Form to open Call center App Ends-->

		<div class="row notificationbar clearfix" style="min-height: 40px;">
			<div class="col-md-2 ">
				
					<div class="sidebar-minified js-toggle-minified" style="height: 0px;">
						<i class="fa fa-bars"></i>

					</div>
				
			</div>


			<form method="post" action="backToSso" id="backToSsoFormId">
			</form>

			<form method="post" action="invalidate" id="logOutSsoFormId">
			</form>

			<div class="col-md-10">
				<!-- <h4 style="position: absolute;margin-top: 0px;">
					<a style="color:white;text-decoration: underline" href="https://emitraapp.rajasthan.gov.in/emitrashared/download/Helpdesk_e-Mitra_V9.pdf" target="_blank">Helpline Numbers <i class="fa fa-download"></i></a>
					&nbsp;
					<a style="color:white;text-decoration: underline" href="https://emitraapp.rajasthan.gov.in/emitrashared/download/Kiosk_Service_Guideline.pdf" target="_blank">Kiosk Service Guideline <i class="fa fa-download"></i></a>
				</h4> -->
	
	
				<marquee direction="left" scrollamount="5" scrolldelay="2" class="NewsClass">
					<span id="headerMarqueeMsg" class="headerMarqueeMsg feed">16-Oct-2023 03:20 PM:-प्रिय ई मित्र कियोस्क धारक, GAYATARI EVERTECH SOLUTIONS PVT LTD विभाग की "ELECTRICITY BILL PAYMENT-POWERED by PJ BILLS" सेवा ई मित्र पोर्टल पर प्रारंभ कर दी गई है। इस सेवा  हेतु कियोस्क को बिजली बिल राशि का 0.30% कमीशन प्राप्त होगा। इस सेवा से संबंधित किसी भी समस्या के लिए निम्न नंबर एवं ई मेल पर संपर्क कर सकते है:-9509069050, Pjbillhelp@gmail.com


12-Oct-2023 12:55 PM:- प्रिय E-MITRA साथियों नमस्कार.... PAYTHROUGH आपके लिए लाई है बेहतर रिचार्ज Facility 🥳🥳🥳🥳🥳🥳🥳🥳🥳
E-MITRA पोर्टल पर मोबाइल रिचार्ज 📱 के लिए हमें संपर्क करें:-
1. VI/ JIO/ AIRTEL/ BSNL की रिचार्ज के लिए PAYTHROUGH रिचार्ज को ही चुनें।
2. टोकन कैंसिलेशन के लिए support@paythrough.in पर mail 💌 करें।
3. रिचार्ज से संबंधित किसी भी समस्या के लिए 8298537537 पर तुरंत संपर्क करें या whatsapp करें। ☺️
4. अपने कीमती सुझाव या अनुभव हमारे टीम के साथ 8298537537 पर whatsapp के जरिए साझा करें। 
5. अपना #support 🤝team paythrough के साथ बनाए रखें।

09-Oct-2023 11:35 AM:-प्रिय ईमित्र कियोस्कधारक, चॉइस नवरात्रि  धमाका कॉन्टेस्ट
प्रिय KIOSK धारक आप जीत सकते है Amazon Voucher और 100 ग्राम चांदी के सिक्के 
इसके लिए आपको केवल चॉइस के डीमैट अकाउंट में निवेश करवाना है😃 
Choice  डीमैट अकाउंट जीरो  टोकन चार्ज पर खोले जाते है  : 0/- 

न्यूनतम 5 डीमैट अकाउंट पर अतिरिक्त 1250 रुपये कमाने का मौका | 


उदहारण KIOSK के लिए :
✅डीमैट अकाउंट ऑफर  
1)  5 डीमैट  अकाउंट, KIOSK को कमीशन 150*5=750  रुपये एवं अक्टूबर ऑफर में पहला निवेश हर खाते में 1500 रुपये का कराये और जीते  500  रुपए  Amazon Voucher, कुल आय = 1250 रुपये
2)  50 डीमैट अकाउंट,  KIOSK को कमीशन 150*50 =7500 रुपये एवं अक्टूबर ऑफर पहला निवेश हर खाते में 1500 रुपये का कराये और जीते 100 ग्राम चांदी का  सिक्का। 
 👉 नोट :-उपरोक्त खातों को खोलना एवं उनमे निवेश करना अनिवार्ये है
        :डीमैट अकाउंट में न्यून्तम  1500  रुपये का  निवेश।  
: अधिक जानकारी के लिए संपर्क करे :6350234013 ,7740998453,�7374870184

04-Oct-2023 06:01 PM:- प्रिय ई मित्र किओस्क धारक, �Sihag Rural Market Private Limited� विभाग की  �Digistall- your gateway to e-commerce� सेवा ई मित्र पोर्टल पर प्रारंभ कर दी गई है। इस सेवा के माध्यम से आप बिना कोड के अपने नजदीकी व्यवसाय की वेबसाइट बना सकते हैं | इसमें कियोस्क को प्रति ट्रांजेक्शन कमीशन - Rs 1200 / - मिलेगा। 

इस सेवा के संबंध में किसी भी प्रकार की सहायता के लिए हेल्पलाइन नंबर- 9461852060 पर संपर्क कर सकते है।

03-Oct-2023 04:45 PM:- प्रिय ई मित्र किओस्क धारक, आवास फाइनेंसियर्स लिमिटेड, होम लोन कम्पनी की "आवास होम लोन लीड जनरेशन" को सेवाएं अब ई मित्र पर उपलब्ध है। आज से ही "आवास होम लोन लीड"दर्ज करना शुरू करें। अधिक जानकारी के लिए आवास ई मित्र पोर्टल लॉगिन करे या हेल्पडेस्क पर संपर्क करे :01413537890 

नोट : "आवास होम लोन लीड जनरेशन" को सेवाएं करोली,धौलपुर, जैसलमेर को छोड़ कर सभी जिलों में उपलब्ध हैं।

01-Oct-2023 02:04 PM:-प्रिय ई मित्र कियोस्क धारक, "Department of Labour" की "Gig Workers Registration" की सेवाएं ई मित्र पोर्टल पर प्रारंभ कर दी गई है।

27-Sep-2023 11:04 AM:-प्रिय ई मित्र कियोस्क धारक,  कृपया कुछ क्षण निकालकर NeSDA द्वारा आयोजित नागरिक सर्वेक्षण में भाग लें। ई-मित्र की राष्ट्र स्तर पर पहचान बनाने के लिए आप का इस सर्वेक्षण में भाग लेना महत्वपूर्ण है।

सर्वेक्षण में भाग लेने के लिए निचे दिए गए लिंक पर क्लिक करें : 
https://nesda.centralindia.cloudapp.azure.com/#/citizen-survey

20-Sep-2023 05:55 PM:-प्रिय ई मित्र कियोस्क धारक, ई मित्र पर उपलब्ध Discom K no Electricity bill pay  (बिजली बिल जमा सेवा) के अतरिक्त किसी अन्य सर्विस  (B2C Partner) से बिजली बिल जमा करने पर रशीद निरस्त करने का प्रावधान नहीं है |

12-Sep-2023 11:56 AM:-प्रिय ई मित्र कियोस्क धारक, ई-मित्र के माध्यम से शाइन ओलंपियाड के फॉर्म भर और जीते आकर्षक इनाम जैसे की कार, मोटरसाइकिल, स्कूटी, लैपटॉप, कलर प्रिंटर, चांदी का सिक्का, स्मार्टफोन आदि। ऑफर 30 सितंबर तक लागू है।
ऑफर 21 अगस्त से शुरू हो चूका है और 30 सितम्बर 2023 तक रहेगा।
300/- रूपये का टोकन और रुपये हर ओलंपियाड पर 99/- कमीशन 
कक्षा 1 से 12 तक स्कूल जाने वाले प्रत्येक छात्र को दिया जा सकता है। 
पूरी जानकारी के लिए Utility में Shine Olympiad टाइप कर सर्विस पर क्लिक करें। या दिए गए नंबर पर कॉल/व्हाट्सप्प करें। 
+91-8448553963

23-Aug-2023 11:00 AM:- प्रिय ई-मित्र कियोस्कधारक, कियोस्क के लिये Grievance Module प्रारम्भ किया जा रहा है, विभाग द्वारा ईमित्र पोर्टल पर आने वाले समस्याओ  से सम्बंधित केटेगरी बना दी गयी है आप निम्न लिंक से यूजर मैन्युअल / ईमित्र पोर्टल के डाउनलोड सेक्नशन से डाउन लोड कर सकते है, 
https://emitraapp.rajasthan.gov.in//emitrashared_2023/USER_MGMT_DOCS/GUIDELINE_AND_EFORM/2023/8/23/GAndE_1692767690518.pdf
आप अपनी समस्याओं के लिए Grievance Module से ही अपनी समस्या बता पायेंगे |    </span>
				</marquee>


				<div class="top-bar-right">
					<!-- responsive menu bar icon -->
					<a href="#" class="hidden-md hidden-lg main-nav-toggle"><i class="fa fa-bars"></i></a>
					<div class="notifications">
						<ul>
							
							<li class="notification-item inbox"><a href="javascript:void(0)" onclick="location.href='dashboard?[B@b996ccc1'" title="Dashboard"><i class="fa fa-home white"></i></a></li>
							
							<!-- Start notification: inbox -->
							 <li class="notification-item general">
								<div class="btn-group">
									<a href="javascript:void(0)" onclick="location.href='myInternalMessages'" class="dropdown-toggle" data-toggle="dropdown">
										<i class="fa fa-envelope"></i>
										<!-- <span class="count hide-service" id="unreadCounterSpan">0</span> 
										<span class="circle"></span> -->
									</a>
									<!-- <ul class="dropdown-menu" role="menu">
										<li><a href="javascript:void(0)" style="cursor:default"> <i class="fa fa-envelope-o" style="color:#EC8239"></i> <span class="text" style="color:black">Unread Message</span> <span class="timestamp" style="color:black" id="unreadCountSpan">0</span> </a></li>
										<li><a href="javascript:void(0)" style="cursor:default"> <i class="fa fa-folder-open-o" style="color:#EC8239"></i> <span class="text" style="color:black">Total Messages</span> <span class="timestamp" style="color:black" id="totalCountSpan">0</span> </a></li>
										<li class="notification-footer"><a href="myInternalMessages">View All Messages</a></li>
									</ul> -->
								</div>
							</li>  
							<!-- end notification: inbox -->
							
							
							
						</ul>
					</div>

					<!-- logged user and the menu -->
					<div class="logged-user">
						<div class="btn-group" style="margin-right: 33px;">
							<a href="#" class="btn btn-link dropdown-toggle" data-toggle="dropdown"> 
									
									
										<img src="resources/assets/images/user-avatar.png" alt="User Avatar" style="float:left; padding-right: 2px;">
									
								 
								<span class="name" style="line-height: 13px; float:left;"> 
								
										MANOJKUMARBALAI813
									
							</span> 
							<br>
						<span style="font-size:10px;"> LSP KIOSK ADMIN</span>
							
							
							
							
							<span class="caret"></span>
							</a>
							<ul class="dropdown-menu" role="menu">
								
								
								<li><a href="javascript:void(0)" onclick="$('#backToSsoFormId').submit()"> <i class="fa fa-home"></i> <span class="text">Back to SSO</span></a></li>
								<li><a href="javascript:void(0)" onclick="$('#logOutSsoFormId').submit()"> <i class="fa fa-power-off"></i> <span class="text">Logout</span></a></li>
							</ul>
						</div>
					</div>
					
					
					
					<a class="btn-sm btn-success hide-service engLangShow" href="javascript:void(0)" onclick="changeAppLanguage('en')" style="display: none;">A</a> 
					<a class="btn-sm btn-success hinLangShow" href="javascript:void(0)" onclick="changeAppLanguage('hi_IN')">अ</a>
					

					<!-- end logged user and the menu -->


				</div>
				<!-- /top-bar-right -->



			</div>
		</div>
		<!-- /row -->
	</div>
	<!-- /container -->
</div>

	
<input type="hidden" id="currentTodayDate" name="time" value="2023-10-19"> 
										
<script>

// A more cryptic one-liner, to awe & impress.
//
// No need to protect `window` since `this` is
// immutable, and at the topmost level means
// `window` anyways. Here, we compare locations
// on the left side of the "&&" and execute the
// code in parenthesis if that condition is
// true (top location isn't iframe location).
//
// Otherwise, nothing happens. It's basically an
// if statement without wrapping curly brackets.
//
// Weird, I know. But pretty cool, right? :)


this.top.location !== this.location && (this.top.location = this.location);


	var curUrl = location.href;		
	curUrl = curUrl.substring(0,curUrl.indexOf('?'));
	if(location.href.indexOf("lang")==-1 && curUrl.indexOf("availServiceEform") != -1){
		$("#langChangeForm").attr("action",curUrl + "?[B@f8145aee");
		$("#langFieldId").val("hi_IN");
		$("#langChangeForm").submit(); 
	}


</script>

		<!-- /TOP BAR -->

		<!-- BOTTOM: LEFT NAV AND RIGHT MAIN CONTENT -->
		<div class="bottom">
			<div class="container">
				<div class="row">

					<!-- left sidebar -->
					<div class="col-md-2 left-sidebar" style="min-height: 751px;">

						<!-- main-nav -->
						

















	<nav class="main-nav">
		<ul class="main-menu" id="menuList">

			<li class="forActive active">
				<a href="javascript:void(0)" class="js-sub-menu-toggle"><i class="fa fa-dashboard fa-fw"></i><span class="text">Home</span> <i class="toggle-icon fa fa-angle-left"></i> </a>
				<ul class="sub-menu nonBreadcrumb active" style="display:block">



				<li class="active"> <a href="dashboard?[B@8fe10210" class="forBreadcrumb"><span class="text">Dashboard</span></a> </li>

				</ul>
			</li>

				


			<li class="forActive">
				<a href="javascript:void(0)" class="js-sub-menu-toggle"><i class="fa fa-check-circle fw"></i><span class="text">Services </span> <i class="toggle-icon fa fa-angle-left"></i> </a>
				<ul class="sub-menu nonBreadcrumb">


					<li> <a href="kioskTransactionList?[B@3f41e76" class="forBreadcrumb"><span class="text">Transaction History</span></a> </li>


					<li> <a href="receiptNoWiseSearch?[B@653c631f" class="forBreadcrumb"><span class="text">Receipt Reprint</span></a> </li>


					<li> <a href="verifyTransaction?[B@66af39a3" class="forBreadcrumb"><span class="text">Verify Pending Transactions</span></a> </li>


					<li> <a href="serviceWorkflowForKioskAndCitizen?[B@d7897cd4" class="forBreadcrumb"><span class="text">Service Workflow For Application Services</span></a> </li>


					<li> <a href="tokenNoWiseSearchJioOtp?[B@509c7d97" class="forBreadcrumb"><span class="text">Check Jio OTP</span></a> </li>


					<li> <a href="pmMaandhanMobReg?[B@1db2385c" class="forBreadcrumb"><span class="text">Mobile Registration For Maandhan Services</span></a> </li>


					<li> <a href="irctcAgentRegistrationForm?[B@afe96c7d" class="forBreadcrumb"><span class="text">Irctc Agent Registration Form</span></a> </li>


					<li> <a href="airtelPrePaid?[B@fc92a06a" class="forBreadcrumb"><span class="text">Airtel Pre Paid Recharge</span></a> </li>


					<li> <a href="hindonUniversityServiceForm?[B@56ef3849" class="forBreadcrumb"><span class="text">Government College Hindaun Fee Deposition</span></a> </li>


					<li> <a href="karauliUniversityServiceForm?[B@afcc51d6" class="forBreadcrumb"><span class="text">KARAULI COLLEGE FEE</span></a> </li>


					<li> <a href="duplicateJamabandiSearch?[B@232db7a3" class="forBreadcrumb"><span class="text">Jamabandi Reprint</span></a> </li>

					<li> <a href="javascript:void(0)" class="js-sub-menu-toggle"> <i class="fa fa-user fw"></i><span class="text">Avail Service</span> <i class="toggle-icon fa fa-angle-left"></i> </a>
						<ul class="sub-menu">

						<li> <a href="availService?[B@e5c1a659" class="forBreadcrumb"><span class="text">Utility</span></a> </li>

						<li> <a href="availServiceEform?[B@d88c110" class="forBreadcrumb"><span class="text">Application</span></a> </li>

							
						</ul>
					</li>

				</ul>
			</li>

				


			<li class="forActive">
				<a href="javascript:void(0)" class="js-sub-menu-toggle"><i class="fa fa-pie-chart fw"></i><span class="text">Financial </span> <i class="toggle-icon fa fa-angle-left"></i> </a>
				<ul class="sub-menu nonBreadcrumb">


					<li> <a href="reconcileFincTransaction?[B@a0c61e86" class="forBreadcrumb"><span class="text">Reconcile Finance Transactions</span></a> </li>

					<li> <a href="javascript:void(0)" class="js-sub-menu-toggle"> <i class="fa fa-user fw"></i><span class="text">Wallet</span> <i class="toggle-icon fa fa-angle-left"></i> </a>
						<ul class="sub-menu">

						<li> <a href="walletDetails?[B@800afd82" class="forBreadcrumb"><span class="text">Wallet Details</span></a> </li>

						<li> <a href="payoutFundForm?[B@da0bfc77" class="forBreadcrumb"><span class="text">Fund Payout</span></a> </li>

						<li> <a href="refillForm?[B@4acb31dc" class="forBreadcrumb"><span class="text">Refill</span></a> </li>

							
						</ul>
					</li>

				</ul>
			</li>

				


			<li class="forActive">
				<a href="javascript:void(0)" class="js-sub-menu-toggle"><i class="fa fa-user fw"></i><span class="text">User Management </span> <i class="toggle-icon fa fa-angle-left"></i> </a>
				<ul class="sub-menu nonBreadcrumb">


					<li> <a href="updateKioskDetails?[B@f2359ebe" class="forBreadcrumb"><span class="text">Kiosk Details</span></a> </li>


					<li> <a href="gspKioskNomination?[B@76541b27" class="forBreadcrumb"><span class="text">GSP Kiosk Nomination</span></a> </li>


					<li> <a href="getKioskIDCard?[B@377b8320" class="forBreadcrumb"><span class="text">id card</span></a> </li>

					<li> <a href="javascript:void(0)" class="js-sub-menu-toggle"> <i class="fa fa-user fw"></i><span class="text">Manage User</span> <i class="toggle-icon fa fa-angle-left"></i> </a>
						<ul class="sub-menu">

						<li> <a href="createKioskUser?[B@54cfa785" class="forBreadcrumb"><span class="text">Create Kiosk User</span></a> </li>

						<li> <a href="kioskMigrationRequest?[B@c837798a" class="forBreadcrumb"><span class="text">Request Migration</span></a> </li>

						<li> <a href="kioskUserPoliceVerification?[B@222927c8" class="forBreadcrumb"><span class="text">Kiosk User Police Verification</span></a> </li>

							
						</ul>
					</li>

				</ul>
			</li>

				

			<li class="forActive">
				<a href="javascript:void(0)" class="js-sub-menu-toggle"><i class="fa fa-wrench fw"></i><span class="text">Tool Management</span> <i class="toggle-icon fa fa-angle-left"></i> </a>
				<ul class="sub-menu nonBreadcrumb">



				<li> <a href="viewAllFavActivities?[B@39570aa0" class="forBreadcrumb"><span class="text">Favorite Pages</span></a> </li>

				</ul>
			</li>

				

			<li class="forActive">
				<a href="javascript:void(0)" class="js-sub-menu-toggle"><i class="fa fa-clipboard fa-fw"></i><span class="text">Inbox</span> <i class="toggle-icon fa fa-angle-left"></i> </a>
				<ul class="sub-menu nonBreadcrumb">



				<li> <a href="viewMyInbox?[B@88627f2" class="forBreadcrumb"><span class="text">View Inbox</span></a> </li>

				</ul>
			</li>

				


			<li class="forActive">
				<a href="javascript:void(0)" class="js-sub-menu-toggle"><i class="fa fa-taxi"></i><span class="text">Travel </span> <i class="toggle-icon fa fa-angle-left"></i> </a>
				<ul class="sub-menu nonBreadcrumb">

					<li> <a href="javascript:void(0)" class="js-sub-menu-toggle"> <i class="fa fa-train"></i><span class="text">IRCTC</span> <i class="toggle-icon fa fa-angle-left"></i> </a>
						<ul class="sub-menu">

						<li> <a href="booking?[B@b7d2fbd3" class="forBreadcrumb"><span class="text">Book Train Ticket</span></a> </li>

						<li> <a href="irctcBookingTicketHistory?[B@919b796d" class="forBreadcrumb"><span class="text">Ticket Booking History</span></a> </li>

						<li> <a href="irctcTicketCancelHistory?[B@2a58d1a4" class="forBreadcrumb"><span class="text">Cancel Ticket History</span></a> </li>

						<li> <a href="irctcFileTdr?[B@494d00b7" class="forBreadcrumb"><span class="text">File TDR</span></a> </li>

							
						</ul>
					</li>

				</ul>
			</li>

				

			<li class="forActive">
				<a href="javascript:void(0)" class="js-sub-menu-toggle"><i class="fa fa-dashboard fa-fw"></i><span class="text">PAN Card - Protean(NSDL)</span> <i class="toggle-icon fa fa-angle-left"></i> </a>
				<ul class="sub-menu nonBreadcrumb">



				<li> <a href="https://emitraapp.rajasthan.gov.in/nsdlapi/oauth/login/?token=K3BRUXJYRHZNaDBSSmQxQWlaZEVab0FBRFVrOTZRSGx1VE9qVnZPVy9KZ0Z2VXBnWkdqWTBOTjZQSHRMVDAyMDEyQnVRSm9rVkdXV1NCRUd0RjJGa2Vwa0RIa2M2eFlkVkZwN254Y3U1RzJoZnFRVEJxTjFZc2FRelBoUnFER2t1QkRPa1dyOFkveW5Ka1BLZ3owZlNUdE94OVhFbHFURTNDa01ESDU3WXUyRmp5b1Z3NGZLVmVMQ2NpZGFzd2Z3" class="forBreadcrumb"><span class="text">PAN Card Service</span></a> </li>

				</ul>
			</li>

				

			<li class="forActive">
				<a href="javascript:void(0)" class="js-sub-menu-toggle"><i class="fa fa-user fw"></i><span class="text">Bank-BC</span> <i class="toggle-icon fa fa-angle-left"></i> </a>
				<ul class="sub-menu nonBreadcrumb">



				<li> <a href="https://emitraapp.rajasthan.gov.in/bankbcapi/oauth/login/?token=K3BRUXJYRHZNaDBSSmQxQWlaZEVab0FBRFVrOTZRSGx1VE9qVnZPVy9KZ0Z2VXBnWkdqWTBOTjZQSHRMVDAyMDEyQnVRSm9rVkdXV1NCRUd0RjJGa2Vwa0RIa2M2eFlkVkZwN254Y3U1RzJoZnFRVEJxTjFZc2FRelBoUnFER2t1QkRPa1dyOFkveW5Ka1BLZ3owZlNUdE94OVhFbHFURTNDa01ESDU3WXUyRmp5b1Z3NGZLVmVMQ2NpZGFzd2Z3" class="forBreadcrumb"><span class="text">Bank BC</span></a> </li>

				</ul>
			</li>

				

			<li class="forActive">
				<a href="javascript:void(0)" class="js-sub-menu-toggle"><i class="fa fa-dashboard fa-fw"></i><span class="text">Grievance Module</span> <i class="toggle-icon fa fa-angle-left"></i> </a>
				<ul class="sub-menu nonBreadcrumb">



				<li> <a href="https://emitraapp.rajasthan.gov.in/grievanceapi/oauth/login/?token=K3BRUXJYRHZNaDBSSmQxQWlaZEVab0FBRFVrOTZRSGx1VE9qVnZPVy9KZ0Z2VXBnWkdqWTBOTjZQSHRMVDAyMDEyQnVRSm9rVkdXV1NCRUd0RjJGa2Vwa0RIa2M2eFlkVkZwN254Y3U1RzJoZnFRVEJxTjFZc2FRelBoUnFER2t1QkRPa1dyOFkveW5Ka1BLZ3owZlNUdE94OVhFbHFURTNDa01ESDU3WXUyRmp5b1Z3NGZLVmVMQ2NpZGFzd2Z3" class="forBreadcrumb"><span class="text">Grievance</span></a> </li>

				</ul>
			</li>

				


		</ul>
	</nav>
	









						<!-- /main-nav -->

						<!-- sidebar content -->
						
						<!-- end sidebar content -->

					</div>
					<!-- end left sidebar -->

					<!-- content-wrapper -->
					<div class="col-md-10 content-wrapper">

						

						<div class="row">
							<!-- Start-breadcrumb -->
							<div class="col-md-2 col-sm-4">
								


	


<ul class="breadcrumb">
	
		<li><i class="fa fa-home"></i><a href="dashboard?[B@52abcadd">Dashboard</a></li>
		
</ul>


							</div>


							<!-- Show it to LSP and Kiosk Only Starts -->
							


							<div class="col-md-10 ">
								<div class="top-content">
									<ul class="list-inline mini-stat">
										<li class="category">
											<h5>
											
												You Are Under Category
												
												
												
												
												
												
													<span class="stat-value stat-color-blue">C</span>
												
											</h5>
										</li>
										<li class="wallet">
											<h5>
												WALLET
												<span class="stat-value stat-color-orange"><i class="fa fa-money"></i> 219.66</span>
											</h5>
										</li>
										<li class="advance">
											<h5>
												ADVANCE
												<span class="stat-value stat-color-blue"><i class="fa fa-inr"></i> 219.66</span>
											</h5>
										</li>
										<li class="creditLimit">
											<h5>
												CREDIT LIMIT
												<span class="stat-value stat-color-seagreen"><i class="fa fa-credit-card"></i> 0.00</span>
											</h5>
										</li>

										

										
											<li class="dues">
												<h5>
													DUES
													<span class="stat-value stat-color-seagreen" id="trigger"><i class="fa fa-minus-square"></i> 0.00</span>
												</h5>
											</li>




										




									</ul>
									
									
									<div class="btn-group col-sm-2 pull-right">
											<a style="width: 93%;" href="refillForm?[B@7a33d63" class="btn btn-primary"> <i class="fa fa-link"></i> Refill Wallet</a>
											
										</div>
									
									
									
									
										
									
								</div>
							</div>
							
							
							<!-- Show it to LSP and Kiosk Only Stop -->
							<!-- End-breadcrumb -->
						</div>
						<div class="row">
							
							

	
	
	&nbsp;
	
							
						</div>

						<div class="content">

							<div class="content">

								<div class="main-content">
								
								
									
																		
								
									
									















<style>
span#blinkText {
	-moz-animation-duration: 400ms;
	-moz-animation-name: blink;
	-moz-animation-iteration-count: infinite;
	-moz-animation-direction: alternate;
	-webkit-animation-duration: 400ms;
	-webkit-animation-name: blink;
	-webkit-animation-iteration-count: infinite;
	-webkit-animation-direction: alternate;
	animation-duration: 400ms;
	animation-name: blink;
	animation-iteration-count: infinite;
	animation-direction: alternate;
}

@
-moz-keyframes blink {from { opacity:1;
	
}

to {
	opacity: 0;
}

}
@
-webkit-keyframes blink {from { opacity:1;
	
}

to {
	opacity: 0;
}

}
@
keyframes blink {from { opacity:1;
	
}

to {
	opacity: 0;
}

}
.rotateText {
	color: red;
	font-weight: 900;
	float: left;
	position: relative;
	width: 50px;
	border-style: none;
	font-size: 20px;
	-webkit-transform: rotate(320deg);
	-moz-transform: rotate(320deg);
	-ms-transform: rotate(320deg);
	-o-transform: rotate(320deg);
	transform: rotate(320deg);
	filter: progid:DXImageTransform.Microsoft.BasicImage(rotation=3);
}

#kiosklinks li{
	
	border-bottom:1px dashed #f1f1f1; 
	padding:10px;
	margin:1px;
	text-align:left;

	
}

table { 
  width: 100%; 
  border-collapse: collapse; 
}
/* Zebra striping */
tr:nth-of-type(odd) { 
  background: #eee; 
}
th { 
  background: #333; 
  color: white; 
  font-weight: bold; 
}
td, th { 
  padding: 0px; 
  border: 1px solid #ccc; 
  text-align: left; 
}


</style>



	<!-- <div class="widget widget-hide-header" id="services">
		<div class="row list-unstyled todo-list" id="service-drag">
		
			<div class="service-box">
				<span class="handle"><i class="fa fa-mobile" id="0001"></i></span>
				<p class="text-center">Recharge</p>
			</div>
		
			<div class="service-box">
				<span class="handle"><i class="fa fa-credit-card" id="0002"></i></span>
				<p class="text-center">Bill Pay</p>
			</div>
			<div class="service-box">
				<span class="handle"><i class="fa fa-inr"></i></span>
				<p class="text-center">Fee Pay</p>
			</div>
			<div class="service-box">
				<span class="handle"><i class="fa fa-book"></i></span>
				<p class="text-center">Education</p>
			</div>
			<div class="service-box">
				<span class="handle"><i class="fa fa-th"></i></span>
				<p class="text-center">Application</p>
			</div>
			<div class="service-box">
				<span class="handle"><i class="fa fa-umbrella"></i></span>
				<p class="text-center">Insurance</p>
			</div>
			<div class="service-box">
				<span class="handle"> <i class="fa fa-ticket"></i></span>
				<p class="text-center">Ticket</p>
			</div>
			<div class="service-box">
				<span class="handle"> <i class="fa fa-mobile"></i></span>
				<p class="text-center">Recharge</p>
			</div>
			<div class="service-box">
				<span class="handle"><i class="fa fa-book"></i></span>
				<p class="text-center">Education</p>
			</div>
			<div class="service-box">
				<span class="handle"><i class="fa fa-th"></i></span>
				<p class="text-center">Application</p>
			</div>
			<div class="service-box">
				<span class="handle"><i class="fa fa-umbrella"></i></span>
				<p class="text-center">Insurance</p>
			</div>
			<div class="service-box">
				<span class="handle"><i class="fa fa-ticket"></i></span>
				<p class="text-center">Ticket</p>
			</div>
			<div class="service-box">
				<span class="handle"><i class="fa fa-mobile"></i></span>
				<p class="text-center">Recharge</p>
			</div>
			<div class="service-box">
				<span class="handle"><i class="fa fa-book"></i></span>
				<p class="text-center">Education</p>
			</div>
		
			<div class="service-box">
				<span class="handle"><i class="fa fa-umbrella"></i></span>
				<p class="text-center">Insurance</p>
			</div>
			<div class="service-box">
				<span class="handle"><i class="fa fa-ticket"></i></span>
				<p class="text-center">Ticket</p>
			</div>
		
		
		
		
		</div>
		
		<div class="servic-data" id="servic-data1">
		
			<div class="service-box">
				<a href="services.html" target="_blank"><i><img
						src="resources/assets/icons/airtel.jpg" class="imgicon"></i></a>
				<p class="text-center">Airtel</p>
			</div>
		
			<div class="service-box">
				<a href="services.html" target="_blank"><i><img
						src="resources/assets/icons/rel.jpg" class="imgicon"></i></a>
				<p class="text-center">Reliance</p>
			</div>
		
			<div class="service-box">
				<a href="services.html" target="_blank"><i><img
						src="resources/assets/icons/idea.jpg"></i></a>
				<p class="text-center">Idea</p>
			</div>
		
			<div class="service-box">
				<a href="services.html" target="_blank"><i><img
						src="resources/assets/icons/bsnl.jpg" class="imgicon"></i></a>
				<p class="text-center">BSNL</p>
			</div>
		
			<div class="service-box">
				<a href="services.html" target="_blank"><i><img
						src="resources/assets/icons/aircel.jpg"></i></a>
				<p class="text-center">Aircel</p>
			</div>
		
			<div class="service-box">
				<a href="services.html" target="_blank"><i><img
						src="resources/assets/icons/vodafone.jpg" class="imgicon"></i></a>
				<p class="text-center">Vodafone</p>
			</div>
		
			<div class="service-box">
				<a href="services.html" target="_blank"><i><img
						src="resources/assets/icons/MTS.jpg"></i></a>
				<p class="text-center">MTS</p>
			</div>
		
		</div>
		
		<div class="servic-data" id="servic-data2">
		
			<div class="service-box">
				<a href="services.html" target="_blank"><i><img
						src="resources/assets/icons/dish.jpg"></i></a>
				<p class="text-center">Dish Tv</p>
			</div>
		
		
			<div class="service-box">
				<a href="services.html" target="_blank"><i><img
						src="resources/assets/icons/tatasky.jpg"></i></a>
				<p class="text-center">Vodafone</p>
			</div>
		
			<div class="service-box">
				<a href="services.html" target="_blank"><i><img
						src="resources/assets/icons/videocon.jpg"></i></a>
				<p class="text-center">MTS</p>
			</div>
		
		</div>
	</div> -->

<!-- Citizen Pending Bill Table 
<div class="col-md-4 pendingBills">
	<div class="widget">
		<div class="widget-header">
			<h3></h3>
			<ul id="pendingBillsid" class="nav nav-tabs pull-right">
				<li class="active"><a href="#serviceTab" data-toggle="tab"><i class="fa fa-user"></i>Services</a></li>
				<li><a href="#recentLog" onclick="buildRecentLogChart()" data-toggle="tab"><i class="fa fa-pie-chart"></i> Recent Log</a></li>
				<li><a href="#myLspCoordinator" onclick="getMyLspCoordinator()" data-toggle="tab">LSP Contact</a></li>
				<li><a href="#pendingBills" data-toggle="tab"><i class="fa fa-user"></i>Pending Bills</a></li> 
			</ul>

		</div>
		<div class="widget-content data-graph-mar ">
			<div class="tab-content no-padding" style="min-height: 220px;">
				<div class="tab-pane fade in" id="pendingBills">
					<table class="table table-striped table-hover no-padding no-margin">
						<thead>
							<tr>
								<th><input type="checkbox"></th>
								<th>Label</th>
								<th>Amount</th>
								<th class="text-center">Action</th>
							</tr>
						</thead>
						<tbody>
							<!-- <tr>
               <td><input type="checkbox"></td>
                 <td>Home</td>
                 <td>5000.00</td>
                 <td class="text-center"><div class="label label-low">ViewBill</div></td>
               </tr>
               
                  <tr>
                   <td><input type="checkbox"></td>
                 <td>Landline Bill</td>
                 <td>2000.00</td>
                 <td class="text-center"><span class="lablefix label-low">ViewBill</span></td>
               </tr>
               
                   <tr>
                   <td><input type="checkbox"></td>
                 <td>Service Bill</td>
                 <td>4000.00</td>
                 <td class="text-center"><span class="lablefix label-low">ViewBill</span></td>
               </tr> 

							<tr>
								<td colspan="4">No Record Found!</td>
							</tr>

						</tbody>
					</table>

					<!-- <button class="btn btn-custom-secondary col-sm-offset-5" data-toggle="modal" data-target="#myModal"><i class="fa fa-rupee"></i> PayNow</button>
           <label class=" label label-danger more col-sm-offset-9">View More</label> 

				</div>
				<div class="tab-pane fade in" id="recentLog"
					style="text-align: center">
					<i class="fa fa-refresh" id="refreshIcon"
						style="font-size: 49px; z-index: 9999; margin-top: 20%"
						onclick="buildRecentLogChart()"></i>
					<!-- <i class="fa fa-pie-chart" id="dummyPie" aria-hidden="true" style="font-size:200px;opacity:0.2;"></i> 
					<div id="chartContainersss" class="hide-service"
						style="width: 300px; height: 200px;"></div>

				</div>
				
				<div class="tab-pane fade in" id="myLspCoordinator" style="height:280px;overflow: auto">
				No Record Found!
				</div>
				
				
				
				<div class="tab-pane fade in active" id="serviceTab">
				<ul>
					
						<li id="utilLi"><a class="forBreadcrumb" href="availService?[B@7857913e">Utility</a></li>
						<li id="appLi"><a class="forBreadcrumb" href="availServiceEform?[B@2ef07f81">Application</a></li>
					
					</ul>
				</div>
				<div class="tab-content no-padding col-sm-12">
					<a href="#" class="dropdown-toggle btn btn-custom-secondary" onclick="initateCerficatePrinting('K12290269')">Download Certificate</a>
				</div>
			</div>
			
		</div>
	</div>
</div>
<!--/ Citizen Pending Bill Table -->


<!-- WIDGET TABBED CONTENT -->
<div class="col-sm-12 tabkisok">

	<div class="widget">
		<div class="widget-header">
			<a href="#" class="dropdown-toggle btn btn-custom-secondary" onclick="initateCerficatePrinting('K12290269')">Download Certificate</a>
			
			<ul id="navtabs" class="nav nav-tabs pull-right">
				<!--<li><a href="#welcomeEmitra" data-toggle="tab"><i
						class="fa fa-home"></i> Message Board</a></li>-->
				<li><a href="#pendingApprovel" onclick="loadUserPendingApproval()" data-toggle="tab"><i class="fa fa-star-half-o"></i> Action request</a></li>
				<li class="active"><a href="#QuickPayDiv" data-toggle="tab" onclick="getQuickPayApps()"><i class="fa fa-user"></i>Quick Services</a></li>
				<li><a href="#FS" data-toggle="tab"><i class="fa fa-thumbs-up"></i> Favorite Service</a></li>
				<li><a href="#FP" onclick="loadUserFavPages()" data-toggle="tab"><i class="fa fa-thumbs-o-up"></i> Favorite Pages</a></li>


			</ul>
			
		</div>
		<div class="widget-content" style="padding: 3px 10px;">
			<div class="tab-content no-padding" style="min-height: 220px; overflow: hidden;">

				<div class="tab-pane fade" id="welcomeEmitra">
					<div class="col-sm-12">
						<div class="container text-center">
						

								
							
						</div>
					</div>
				</div>

				<div class="tab-pane fade in active" id="QuickPayDiv">
				
				<div class="widget" style="border:none; padding:0; margin:0;">

				<div class="widget-content" style="padding:2px;" id="QuickPay">				
					 
					 
				</div>

				<div class="widget-footer text-right" style="padding: 3px;">				
				<a style="background-color: #ec8239; border-color: #e49626;" href="availServiceEform?[B@1488302a" class="btn btn-warning"> <i class="fa fa-newspaper-o"></i> Application Type Services</a>	
				
				
				<a class="btn btn-primary" href="availService?[B@b94c3e6c"> <i class="fa fa-cubes"></i> Utility Type Services</a>					
					 
				</div>					
					
					
					
				</div>
				</div>
				
				
				
				<div class="tab-pane fade" id="FS">
					<ul id="dragdrop-todo" class="list-unstyled todo-list ui-sortable">
                          <li> <span class="list-control"> <span class="handle"><i class="fa fa-bars"></i></span> </span>
                            <p> <strong>Bhamashah Enrollment, Seeding, Secondary Entry</strong><a href="availService?favSrvId=1248"><span class="label label-danger">Open</span></a> </p>
                          </li>
                          <li> <span class="list-control"> <span class="handle"><i class="fa fa-bars"></i></span> </span>
                            <p> <strong>New Ration Card Form Filling (Form 1)</strong><a href="availService?favSrvId=1622"><span class="label label-danger">Open</span></a> </p>
                          </li>
                          <li> <span class="list-control"> <span class="handle"><i class="fa fa-bars"></i></span> </span>
                            <p> <strong>Ration Card Add Name/ Deletion Of Name/ Correction (Form - 4)</strong><a href="availService?favSrvId=1642"><span class="label label-danger">Open</span></a> </p>
                          </li>
                          <li> <span class="list-control"> <span class="handle"><i class="fa fa-bars"></i></span> </span>
                            <p> <strong>Ration Card Cancellation (Form - 5)</strong><a href="availService?favSrvId=1643"><span class="label label-danger">Open</span></a> </p>
                          </li>
                          <li> <span class="list-control"> <span class="handle"><i class="fa fa-bars"></i></span> </span>
                            <p> <strong>Ration Card Transfer to other Village/ BDO/ District (Form - 7)</strong><a href="availService?favSrvId=1644"><span class="label label-danger">Open</span></a> </p>
                          </li>
                          <li> <span class="list-control"> <span class="handle"><i class="fa fa-bars"></i></span> </span>
                            <p> <strong>Duplicate Ration Card (Form - 6)</strong><a href="availService?favSrvId=1662"><span class="label label-danger">Open</span></a> </p>
                          </li>
                          <li> <span class="list-control"> <span class="handle"><i class="fa fa-bars"></i></span> </span>
                            <p> <strong>Ration Card Other State Transfer (Form-9)</strong><a href="availService?favSrvId=1663"><span class="label label-danger">Open</span></a> </p>
                          </li>
                          <li> <span class="list-control"> <span class="handle"><i class="fa fa-bars"></i></span> </span>
                            <p> <strong>RTI Application Form Submission</strong><a href="availService?favSrvId=1683"><span class="label label-danger">Open</span></a> </p>
                          </li> 
                          <li> <span class="list-control"> <span class="handle"><i class="fa fa-bars"></i></span> </span>
                            <p> <strong>RTI Fee Deposition for Dissemination of Information</strong><a href="availService?favSrvId=1684"><span class="label label-danger">Open</span></a> </p>
                          </li>
                          <li> <span class="list-control"> <span class="handle"><i class="fa fa-bars"></i></span> </span>
                            <p> <strong>RSMSSB Recruitment for Junior Instructor</strong><a href="availService?favSrvId=1768"><span class="label label-danger">Open</span></a> </p>
                          </li> 
                          <li> <span class="list-control"> <span class="handle"><i class="fa fa-bars"></i></span> </span>
                            <p> <strong>RSMSSB Direct Joint Recruitment for Lab Assistant Exam -2016</strong><a href="availService?favSrvId=1769"><span class="label label-danger">Open</span></a> </p>
                          </li>                         
                        </ul>
					
				</div>
				<div class="tab-pane fade" id="FP">
					




<ul id="dragdrop-todo-FP" class="list-unstyled todo-list">
</ul>

<span class="btn btn-custom-primary pull-right" onclick="location.href='viewAllFavActivities'">Show All</span>



	

				</div>

				<div class="tab-pane fade" id="pendingApprovel">

					<div class="col-sm-12">
						<div id="pendingActi">

							




<div class="widget-header">
	<h3>Action request to process other pending activity</h3>

	<div class="btn-group widget-header-toolbar">
		<a data-toggle="collapse" class="btn-borderless " href="#collapsetwo"> <i class="fa fa-chevron-up"></i>
		</a>
	</div>

</div>



<form id="view-dept-kiosk-master-entry" accept-charset="ISO-8859-1" action="viewDeptKioskRegistration" method="post">
	<input type="hidden" name="vendorProfileDetailId" id="vendorProfileDetailDeptKioskId">
	<input type="hidden" name="workflowCall" value="Y">
	<input type="hidden" name="regWorkflowLvlId" id="regWorkflowLvlDeptKioskRegId">
</form>

<form id="view-lsp-kiosk-master-entry" accept-charset="ISO-8859-1" action="viewLspKioskRegistration" method="post">
	<input type="hidden" name="vendorProfileDetailId" id="vendorProfileDetailLspKioskId">
	<input type="hidden" name="workflowCall" value="Y">
	<input type="hidden" name="regWorkflowLvlId" id="regWorkflowLvlLspKioskRegId">
</form>

<form id="view-lsp-master-entry" accept-charset="ISO-8859-1" action="viewLspRegistration" method="post">
	<input type="hidden" name="vendorProfileDetailId" id="vendorProfileDetailLspId">
	<input type="hidden" name="workflowCall" value="Y">
	<input type="hidden" name="regWorkflowLvlId" id="regWorkflowLvlLspRegId">
</form>

<div id="collapsetwo" class="panel-collapse active">
	<div class="table-responsive">
		<table class="table table-sorting table-striped table-hover datatable pendingApprovelTable">
			<thead>
				<tr>
					<th>S. No.</th>
					<th>Request Id</th>
					<th>Entity Name</th>
					<th>Application for GSP</th>
					<th>Is Paypoint</th>
					<th>Bank BC</th>
					<th>Govt. Premises</th>
					
					<th>LSP / Department</th>
					<th>District</th>
					
					<th>Old Kiosk Code</th>
					<th>Purpose</th>
					<th>Registration Date</th>
					<th>Initiation Date</th>
					<th>Initiated By </th>
					<th>Status</th>
					<th>Action</th>
				</tr>
			</thead>
			<tbody id="activityInboxTbody">
			</tbody>
		</table>
		<span class="btn btn-custom-primary pull-right" onclick="location.href='viewMyInbox'">Show All</span>
	</div>
</div>


<script>
	function showActivityInboxDetails(vendorProfileIdValue,entityTypeIdValue,purpose,regWorkflowLevelId){
		
		
		if(entityTypeIdValue == 4){
			
			if(purpose == "LSP REGISTRATION"){
				$("#vendorProfileDetailLspId").val(vendorProfileIdValue);
				$("#regWorkflowLvlLspRegId").val(regWorkflowLevelId);
				$("#view-lsp-master-entry").submit();
			}
			else if(purpose == "LSP  MIGRATION"){
				
			}
			else if(purpose == "LSP  RELOCATION"){
				
			}
			else if(purpose == "LSP  CLOSURE/WITHDRAWAL"){
		
			}
			
		}
		else if(entityTypeIdValue == 5){
			if(purpose == "LSP KIOSK REGISTRATION"){
				$("#vendorProfileDetailLspKioskId").val(vendorProfileIdValue);
				$("#regWorkflowLvlLspKioskRegId").val(regWorkflowLevelId);
				$("#view-lsp-kiosk-master-entry").submit();
			}
			else if(purpose == "4  MIGRATION"){
				
			}
			else if(purpose == "4  RELOCATION"){
				
			}
			else if(purpose == "4  CLOSURE/WITHDRAWAL"){
		
			}
			
		}
		else if(entityTypeIdValue == 6){
			if(purpose == "DEPARTMENT KIOSK REGISTRATION"){
				
				$("#vendorProfileDetailDeptKioskId").val(vendorProfileIdValue);
				$("#regWorkflowLvlDeptKioskRegId").val(regWorkflowLevelId);
				$("#view-dept-kiosk-master-entry").submit();
			}
			else if(purpose == "4  MIGRATION"){
				
			}
			else if(purpose == "4  RELOCATION"){
				
			}
			else if(purpose == "4  CLOSURE/WITHDRAWAL"){
		
			}
			
		}
		else if(entityTypeIdValue == 7){
			if(purpose == "INDEPENDENT KIOSK REGISTRATION"){
				$("#vendorProfileDetailLspKioskId").val(vendorProfileIdValue);
				$("#regWorkflowLvlLspKioskRegId").val(regWorkflowLevelId);
				$("#view-lsp-kiosk-master-entry").submit();
			}
			else if(purpose == "4  MIGRATION"){
				
			}
			else if(purpose == "4  RELOCATION"){
				
			}
			else if(purpose == "4  CLOSURE/WITHDRAWAL"){
		
			}
			
		}
		if(purpose == "REGISTRATION"){
			
		}
		else if(purpose == "MIGRATION"){
			
			
		}
		else if(purpose == "RELOCATION"){
			
			
		}
		else if(purpose == "CLOSURE/WITHDRAWAL"){
	
		}
	}
</script>

						</div>
						

					</div>
				</div>
			</div>
		</div>

	</div>
	
	
	<div class="widget">
		<div class="widget-header"><h3 class="toggle">Reports</h3></div>
	<div class="widget-content container text-center" id="kioskRep">
	
	
	<div class="service-box" id="transactionhistory" style="width: 18%;"><a class="linktxt" href="kioskTransactionList?ru6pxg#"><i class="fa fa-arrows-h reportBox"></i><p class="text-center reportboxTitle">Transaction History</p></a></div><div class="service-box" id="serviceworkflowforapplicationservices" style="width: 18%;"><a class="linktxt" href="serviceWorkflowForKioskAndCitizen?rsylt9#"><i class="fa fa-circle-o-notch reportBox"></i><p class="text-center reportboxTitle">Service Workflow For Application Services </p></a></div><div class="service-box" id="receiptreprint" style="width: 18%;"><a class="linktxt" href="receiptNoWiseSearch?fd54je#"><i class="fa fa-newspaper-o reportBox"></i><p class="text-center reportboxTitle">Receipt Reprint</p></a></div><div class="service-box" id="transactiontrailsummaryreport" style="width:18%; display:none;"><a class="linktxt" href="transactionTrailSummaryReport?gft0dk#"><i class="fa fa-credit-card reportBox"></i><p class="text-center reportboxTitle">Transaction Trail Summary Report</p></a></div><div class="service-box" id="servicewisekioskcommissionsharereport" style="width:18%; display:none;"><a class="linktxt" href="jasperServiceKioskWiseCommReport?knsdk5#"><i class="fa fa-diamond reportBox"></i><p class="text-center reportboxTitle">Service Wise Kiosk Commission Share Report</p></a></div></div>
	</div>

	
	
	
	<div class="widget">
		<div class="widget-header"><h3 class="toggle">Message Board</h3></div>
	<div class="widget-content container text-center">
	<br>
 
 
						
							
							<h1> Welcome to New Emitra </h1> <span style="font-weight: bold;color:red">ऑनलाइन आवेदन करने वाले आवेदकों के लिये होम डिलीवरी की सर्विस प्रारम्भ कर दी गयी है|</span><br> <span style="font-weight: bold;">Dear Kiosk, </span> <br> <span style="color:black"></span><span style="font-weight: bold">ई-मित्र पर सभी प्रकार के प्रमाण पत्रों की सेवाएं Online Users के लिए प्रारम्भ कर दी गयी है | जारी किए गए प्रमाण पत्र को Approve तथा Digital Signature का SMS आपके मोबाइल पर प्राप्त होने के पश्चात आप अपने नजदीकी ई-मित्र पर निर्धारित शुल्क देकर भी प्राप्त कर सकते है अथवा आप अपने निवास स्थान पर भी बिना अतिरिक्त शुल्क के प्राप्त कर सकते है| अपने निवास स्थान पर प्राप्त करने हेतु कृपया Avail Service में जाकर Certificate Home Delivery Service का चयन कर निर्धारित राशि का भुगतान कर दे|</span><br><span><b>Please delete your browser history before logging in e-Mitra on regular basis!</b><br><a href="https://emitraapp.rajasthan.gov.in/emitrashared/logo/Blacklist_120cc_Ad_27_March_2018.pdf" target="_blank" style="color:red">ई-मित्र परियोजना के तहत कार्यरत ई- मित्रा कियोस्कों द्वारा आमजन से धोखाधड़ी एवं वित्त्तीय अनियमितता करने के कारण स्थायी रूप से निष्कासित/बन्द (ब्लैकलिस्ट) किया गया है इन कियोस्कों के विरुद्ध विभाग द्वारा एफआईआर दर्ज करवा दी गयी है अत: इन ई- मित्रा कियोस्कों से ई- मित्रा पर उपलब्ध सेवाओं से सम्बन्धित किसी भी प्रकार का लेन-देन नहीं करें</a></span>
							
							<br><br>
							
							<p style="text-align:left;color:red"><b><span style="color:red">*Note</span>: मूल निवास, जाति प्रमाण पत्र तथा ऐसी अन्य सभी सेवाये जिनमे प्रमाण पत्र जारी किये जाते हैं उन सभी के प्रमाण पत्र का प्रिंट Avail Service में जा कर Print Certificate की सेवा के माध्यम से लेवें|<br>
							(यह सेवा पहले Print Bonafide Certificate के नाम से दी जा रही थी, अब यह Print Certificate के नाम से उपलब्ध है)</b>
							</p>
							
							<ul id="kiosklinks">
  <li class="list-group-item"> <i class="fa fa-chevron-right" aria-hidden="true"></i> <a href="https://emitraapp.rajasthan.gov.in/emitrashared/Morpho_Driver/Morpho_Driver.rar">Download Morpho Driver For UID Mobile Number Updated Service</a></li>
  <li class="list-group-item"> <i class="fa fa-chevron-right" aria-hidden="true"></i> <a href="https://emitraapp.rajasthan.gov.in/emitrashared/logo/PVCPRINTSETUP_V13.zip">Download PVC Print Setup And Guideline</a></li>
   <li class="list-group-item"> <i class="fa fa-chevron-right" aria-hidden="true"></i> <a href="https://emitraapp.rajasthan.gov.in/emitrashared/logo/TeamViewerQS.exe">Download TeamViewer Quick Support V11</a></li>
  

</ul>
							
							
							
							
						
							
							
							
							
							<br>		
								
							
								<div id="bgpara" style="display: none;">
								
								</div>
								<p style="text-align:left;" id="headerMarqueeMsg" class="headerMarqueeMsg">16-Oct-2023 03:20 PM:-प्रिय ई मित्र कियोस्क धारक, GAYATARI EVERTECH SOLUTIONS PVT LTD विभाग की "ELECTRICITY BILL PAYMENT-POWERED by PJ BILLS" सेवा ई मित्र पोर्टल पर प्रारंभ कर दी गई है। इस सेवा  हेतु कियोस्क को बिजली बिल राशि का 0.30% कमीशन प्राप्त होगा। इस सेवा से संबंधित किसी भी समस्या के लिए निम्न नंबर एवं ई मेल पर संपर्क कर सकते है:-9509069050, Pjbillhelp@gmail.com


12-Oct-2023 12:55 PM:- प्रिय E-MITRA साथियों नमस्कार.... PAYTHROUGH आपके लिए लाई है बेहतर रिचार्ज Facility 🥳🥳🥳🥳🥳🥳🥳🥳🥳
E-MITRA पोर्टल पर मोबाइल रिचार्ज 📱 के लिए हमें संपर्क करें:-
1. VI/ JIO/ AIRTEL/ BSNL की रिचार्ज के लिए PAYTHROUGH रिचार्ज को ही चुनें।
2. टोकन कैंसिलेशन के लिए support@paythrough.in पर mail 💌 करें।
3. रिचार्ज से संबंधित किसी भी समस्या के लिए 8298537537 पर तुरंत संपर्क करें या whatsapp करें। ☺️
4. अपने कीमती सुझाव या अनुभव हमारे टीम के साथ 8298537537 पर whatsapp के जरिए साझा करें। 
5. अपना #support 🤝team paythrough के साथ बनाए रखें।

09-Oct-2023 11:35 AM:-प्रिय ईमित्र कियोस्कधारक, चॉइस नवरात्रि  धमाका कॉन्टेस्ट
प्रिय KIOSK धारक आप जीत सकते है Amazon Voucher और 100 ग्राम चांदी के सिक्के 
इसके लिए आपको केवल चॉइस के डीमैट अकाउंट में निवेश करवाना है😃 
Choice  डीमैट अकाउंट जीरो  टोकन चार्ज पर खोले जाते है  : 0/- 

न्यूनतम 5 डीमैट अकाउंट पर अतिरिक्त 1250 रुपये कमाने का मौका | 


उदहारण KIOSK के लिए :
✅डीमैट अकाउंट ऑफर  
1)  5 डीमैट  अकाउंट, KIOSK को कमीशन 150*5=750  रुपये एवं अक्टूबर ऑफर में पहला निवेश हर खाते में 1500 रुपये का कराये और जीते  500  रुपए  Amazon Voucher, कुल आय = 1250 रुपये
2)  50 डीमैट अकाउंट,  KIOSK को कमीशन 150*50 =7500 रुपये एवं अक्टूबर ऑफर पहला निवेश हर खाते में 1500 रुपये का कराये और जीते 100 ग्राम चांदी का  सिक्का। 
 👉 नोट :-उपरोक्त खातों को खोलना एवं उनमे निवेश करना अनिवार्ये है
        :डीमैट अकाउंट में न्यून्तम  1500  रुपये का  निवेश।  
: अधिक जानकारी के लिए संपर्क करे :6350234013 ,7740998453,�7374870184

04-Oct-2023 06:01 PM:- प्रिय ई मित्र किओस्क धारक, �Sihag Rural Market Private Limited� विभाग की  �Digistall- your gateway to e-commerce� सेवा ई मित्र पोर्टल पर प्रारंभ कर दी गई है। इस सेवा के माध्यम से आप बिना कोड के अपने नजदीकी व्यवसाय की वेबसाइट बना सकते हैं | इसमें कियोस्क को प्रति ट्रांजेक्शन कमीशन - Rs 1200 / - मिलेगा। 

इस सेवा के संबंध में किसी भी प्रकार की सहायता के लिए हेल्पलाइन नंबर- 9461852060 पर संपर्क कर सकते है।

03-Oct-2023 04:45 PM:- प्रिय ई मित्र किओस्क धारक, आवास फाइनेंसियर्स लिमिटेड, होम लोन कम्पनी की "आवास होम लोन लीड जनरेशन" को सेवाएं अब ई मित्र पर उपलब्ध है। आज से ही "आवास होम लोन लीड"दर्ज करना शुरू करें। अधिक जानकारी के लिए आवास ई मित्र पोर्टल लॉगिन करे या हेल्पडेस्क पर संपर्क करे :01413537890 

नोट : "आवास होम लोन लीड जनरेशन" को सेवाएं करोली,धौलपुर, जैसलमेर को छोड़ कर सभी जिलों में उपलब्ध हैं।

01-Oct-2023 02:04 PM:-प्रिय ई मित्र कियोस्क धारक, "Department of Labour" की "Gig Workers Registration" की सेवाएं ई मित्र पोर्टल पर प्रारंभ कर दी गई है।

27-Sep-2023 11:04 AM:-प्रिय ई मित्र कियोस्क धारक,  कृपया कुछ क्षण निकालकर NeSDA द्वारा आयोजित नागरिक सर्वेक्षण में भाग लें। ई-मित्र की राष्ट्र स्तर पर पहचान बनाने के लिए आप का इस सर्वेक्षण में भाग लेना महत्वपूर्ण है।

सर्वेक्षण में भाग लेने के लिए निचे दिए गए लिंक पर क्लिक करें : 
https://nesda.centralindia.cloudapp.azure.com/#/citizen-survey

20-Sep-2023 05:55 PM:-प्रिय ई मित्र कियोस्क धारक, ई मित्र पर उपलब्ध Discom K no Electricity bill pay  (बिजली बिल जमा सेवा) के अतरिक्त किसी अन्य सर्विस  (B2C Partner) से बिजली बिल जमा करने पर रशीद निरस्त करने का प्रावधान नहीं है |

12-Sep-2023 11:56 AM:-प्रिय ई मित्र कियोस्क धारक, ई-मित्र के माध्यम से शाइन ओलंपियाड के फॉर्म भर और जीते आकर्षक इनाम जैसे की कार, मोटरसाइकिल, स्कूटी, लैपटॉप, कलर प्रिंटर, चांदी का सिक्का, स्मार्टफोन आदि। ऑफर 30 सितंबर तक लागू है।
ऑफर 21 अगस्त से शुरू हो चूका है और 30 सितम्बर 2023 तक रहेगा।
300/- रूपये का टोकन और रुपये हर ओलंपियाड पर 99/- कमीशन 
कक्षा 1 से 12 तक स्कूल जाने वाले प्रत्येक छात्र को दिया जा सकता है। 
पूरी जानकारी के लिए Utility में Shine Olympiad टाइप कर सर्विस पर क्लिक करें। या दिए गए नंबर पर कॉल/व्हाट्सप्प करें। 
+91-8448553963

23-Aug-2023 11:00 AM:- प्रिय ई-मित्र कियोस्कधारक, कियोस्क के लिये Grievance Module प्रारम्भ किया जा रहा है, विभाग द्वारा ईमित्र पोर्टल पर आने वाले समस्याओ  से सम्बंधित केटेगरी बना दी गयी है आप निम्न लिंक से यूजर मैन्युअल / ईमित्र पोर्टल के डाउनलोड सेक्नशन से डाउन लोड कर सकते है, 
https://emitraapp.rajasthan.gov.in//emitrashared_2023/USER_MGMT_DOCS/GUIDELINE_AND_EFORM/2023/8/23/GAndE_1692767690518.pdf
आप अपनी समस्याओं के लिए Grievance Module से ही अपनी समस्या बता पायेंगे |    </p>
								
</div>
</div>
	
	
	
</div>

<!-- Certificate Printing Starts -->
<div id="lspKioskCertificatePrinting" class="modal fade" role="dialog">
	<div class="modal-dialog modal-dialog" style="width: 80%; background: white" id="modelCertificatePrint">
		<!-- Modal content-->
		<div class="modal-dialog" style="width: 80%; background: #fff; padding: 5px;">
			<div class="modal-header">
				<button type="button" class="close" data-dismiss="modal">×</button>
			</div>
			<!-- Modal content-->
			<div id="certificateModelBody" class="modal-body" style="padding: 0px 10px 0px 10px;">
				<div style="width: 100%; clear: both;" id="certificateHeaderDiv" name="certificateHeaderDiv">
					<div style="width: 25%; float: left;">
						<img class="img-square" src="resources/assets/images/t-logo.png">
					</div>

					<div style="width: 50%; float: left; text-align: center;">
						<div>
							<h4>राजस्थान सरकार</h4>
							<h4>
								जिला ई मित्र सोसाइटी <span id="certHinDistSpan"></span>
							</h4>
							<h4>
								<strong>ई मित्र कियोस्क धारक प्रमाण-पत्र </strong>
							</h4>
						</div>
					</div>
					<div style="width: 25%; float: left;">
						<img id="certUsrImgCertificate" class="img-square" height="100" width="100" src="resources/assets/images/default_profile.jpg" style="border: 1px solid #333;">
					</div>
				</div>

				<div style="width: 100%; clear: both;">
					<p>
						प्रमाणित किया जाता है की श्री/सुश्री/श्रीमती "<strong><span id="certKioskAdminName"></span></strong>" निवासी "<strong><span id="certKioskRegAddress"></span></strong>" को ई गवर्नेंस योजना के तहत
						खोले जाने वाले ई मित्र सेवा का सेवा केंद्र एजेंसी ( <strong><span class="certLspNameSpan"></span></strong>) द्वारा चयन किया जाता है |
					</p>
					<p>
						ई मित्र कियोस्क संख्या "<strong><span id="certKioskCode"></span></strong>"
						में विभिन्न स्वीकृत नागरीकोन्मुखी सरकारी सेवाये ( <strong>G2C</strong>
						) अथवा नागरीकोन्मुखी व्यावस्यीक सेवाये ( <strong>B2C</strong> )
						कि ई मित्र मे उल्लेखित है, को जनता को उपलब्ध कराने हेतु राजस्थान
						के "<strong><span id="certKioskPropAddress"></span></strong>" मे
						<strong><span class="certLspNameSpan"></span></strong> व <strong><span class="certKioskNameSpan"></span></strong> के मध्य की निविदा शर्तो के तहत
						संचालन हेतु अधिकृत किया जाता है|
					</p>
					<p>यह प्रमाण-पत्र इस परियोजना के सभी पक्षकारो के मध्य हुई
						शर्तो के अनुरूप संचालन होने की अवस्था मे जारी होने की दिनाक से
						मान्य रहेगा |</p>
				</div>



				<div style="padding: 20px;">
					<div style="width: 13%; float: left;">
						<b>स्वीकृति दिनांक</b><br> <span id="approvedDate"></span>
					</div>
					<div style="width: 11%; float: left;">
						<b>प्रिंट दिनांक</b><br> <span id="certIssueDate">19/10/2023</span>
					</div>
					<div style="width: 40%; float: left;">
						<b>वर्तमान स्थिति</b><br> <span id="currStatus"></span>
					</div>
					<div style="width: 35%; float: left; text-align: right;">
						<b><span id="approverDeptName"></span></b><br>जारीकर्ता
					</div>
				</div>
			</div>

			<div style="border-top: 1px solid #D8D8D8; padding-top: 10px; width: 100%; clear: both; margin-top: 20px; text-align: right;">This
				is computer generated Certificate</div>
		</div>
		<div class="modal-footer modal-footer">
			<button type="button" class="btn-sm invoiceView printButton" data-print="Y">
				<i class="fa fa-print"></i> Print
			</button>
		</div>
	</div>
</div>
<!-- Certificate Printing Ends -->


<div id="emitraPlusKioskMsgModal" class="modal fade confirm" role="dialog" style="z-index: 99999999">
	<div class="modal-dialog" style="width:60%;">

		<!-- Modal content-->
		<div class="modal-content oh" style="border-radius: 8px">
			<div class="modal-body" style="border: 4px solid #EC8239; border-radius: 8px">
	<!--<div style="color:blue;font-size: 12px;">			
<p >				
<h3>ई-मित्र प्लस मशीनों पर ब्रॉडकास्ट की प्रक्रिया - </h3>
<h4>सभी ई-मित्र प्लस मशीनों पर ब्रॉडकास्ट किये जाने की Testing हेतु निम्नानुसार मशीन को ऑपरेट कराया जाना सुनिश्चित करें :- </h4>
<ul>
<li>ई-मित्र प्लस मशीन ऑन (चालू) होना सुनिश्चित करें।</li>
<li>ई-मित्र प्लस मशीन  पर उपलब्ध विकल्प हिन्दी / English का चयन करें।</li>
<li><शुरू करने के लिए> / <Click To Begin> का चयन करें।</li>
<li><वीसी और वेबकास्ट> / <VC & Webcast> का चयन करें।</li>
<li><बायोस्कोप/वेबकास्ट> <यूट्यूब> <वीएलसी> / <Bioscope/Webcast> <Youtube> <VLC>  विकल्प में से < बायोस्कोप/वेबकास्ट > / <Bioscope/Webcast> का चयन करें।</li>
<li>उक्त विकल्पों के चयन के उपरान्त Official Webcast Portal, Government of Rajasthan खुल जायेगा। </li>
</ul>
</p>

<p >
<h3>ग्रामीण ई-मित्र प्लस मशीनों पर वीडियो कांफ्रान्सिंग (VC) करने की प्रक्रिया -</h3>
<h4>ग्रामीण ई-मित्र प्लस मशीनों पर वीडियो कांफ्रान्सिंग (VC) से संवाद किये जाने की Testing हेतु निम्नानुसार मशीन  को ऑपरेट कराया जाना सुनिश्चित करें:-</h4>
<ul>
<li>ई-मित्र प्लस मशीन  ऑन (चालू) होना सुनिश्चित करें।</li>
<li>ई-मित्र प्लस मशीन  पर उपलब्ध विकल्प हिन्दी / English का चयन करें।</li>
<li><शुरू करने के लिए> / <Click To Begin> का चयन करें।</li>
<li><वीसी और वेबकास्ट> / <VC & Webcast> का चयन करें।</li>
<li>< बायोस्कोप/वेबकास्ट > <यूट्यूब> <वीएलसी> <वीसी (वेबेक्स)> <वीसी (गूगल)> <वीसी (जूम)> / <Bioscope/Webcast> <Youtube> <VLC> <VC(Webex)> <VC(Google)> <VC (Zoom)>  विकल्प में से <वीसी (वेबेक्स)> / <VC (Webex)> का चयन करें।</li>
<li> उक्त विकल्पों के चयन के उपरान्त Webex VC चालू हो जायेगी। </li>
</p>


</div>-->

<div style="color:blue;font-size: 14px;">
<p>प्रिय कीओस्क, SJE (समाज कल्याण विभाग) द्वारा पेंशन प्राप्त करने वाले पेंशनर वार्षिक पेंशन सत्यापन की सेवा ई-मित्र प्लस मशीनों पर  निःशुल्क उपलब्ध है जबकि ई-मित्र पर 50 रुपए शुल्क है। सत्यापन के बाद में ई-मित्र प्लीस मशीन पर उपलब्ध्  Raj SSP  विकल्पक का उपयोग करके पेंशनर को सत्यापन का सर्टिफिकेट अवश्य प्रिंट करके देवे, ईमित्र प्लस मशीन पर सर्टिफिकेट प्रिंट का शुल्क रुपए 10 मात्र ही है,  ईमित्र प्ल स मशीनों पर अधिक से अधिक आमजन को  ट्रांजेक्शन करवाना सुनिश्चित करावें।</p>
</div>				
				
				
				<p>
				</p><div id="commonAlertMessageDiv" class="text-justify"><span style="color:black;font-size: 12px;" id="tempPlusMsg">
				<p>
				
				</p><h3>ई-मित्र प्लस मशीन पर उपलब्ध प्रमुख सेवाएँ –</h3>
<ul id="kli">
<li>सामाजिक सुरक्षा पेंशनर्स का वार्षिक बायोमेट्रिक सत्यापन (निःशुल्क) </li>
<li>जनआधार में मोबाइल नंबर जोड़ना एवं संशोधन करना (निःशुल्क)</li>
<li>ई-आधार एवं ई-जनआधार कार्ड का प्रिन्ट </li>
<li>प्रमाण-पत्र प्रिन्ट (जाति/मूल/विवाह/जन्म/मृत्यु आदि)</li>
<li>बिल भुगतान (बिजली/पानी/मोबाइल आदि)</li>
<li>जमाबंदी एवं गिरदावरी की प्रमाणित (डिजिटल हस्ताक्षर) नक़ल प्रिन्ट</li>
</ul>

				
				
				<p></p>
				<br>

</span>
<p>
आपका किओस्क ई-मित्र प्लस मशीन से मैप है। New eMitra SLA के अनुसार ई-मित्र प्लस मशीन पर मैप किओस्क ऑपरेटर की बायोमेट्रिक उपस्थिति निम्नानुसार दर्ज करना अनिवार्य है :-<br>

 </p><p class="text-center"><b>ई-मित्र प्लस के लिये वान्छनीय न्यूनतम बायोमेट्रिक उपस्थिति </b> </p>

<p></p>

<p>
</p><table id="ktab" cellspacing="0" cellpadding="0" style="padding:0; margin:0; ">
<tbody><tr>
<td width="155" style="text-align:center;"><br>
माह </td>
<td width="200"><p align="center">कोलोकेटेड (ईमित्र प्लस मशीन एंव ई-मित्र किऑस्क एक ही    परिसर में) ई-मित्र प्लस के लिये वान्छनीय न्यूनतम बायोमेट्रिक उपस्थिति  </p></td>
<td width="252"><p align="center">नॉन-कोलोकेटेड (ई-मित्र प्लस मशीन एंव ई-मित्र    किऑस्क अलग अलग जगह पर) ई-मित्र प्लस के लिये वान्छनीय न्यूनतम बायोमेट्रिक उपस्थिति </p></td>
</tr>
<tr>
<td width="155" nowrap=""><p align="center"> जनवरी-2022 एंव इसके बाद </p></td>
<td width="200" nowrap=""><p align="center">12</p></td>
<td width="252" nowrap=""><p align="center">08</p></td>
</tr>
</tbody></table>



<p></p>
<p>
किसी माह में उक्त तालिका के अनुसार उपस्थिति कम पाये जाने पर 500 रुपये की शास्ति आरोपित की जावेगी (Kiosk : 375 रुपये एवं LSP :125 रुपये) । यदि आपको ई-मित्र प्लस मशीन पर कीओस्क ऑपरेटर की उपस्थिति दर्ज करने में कोई समस्या है तो सहायता हेतु SSO Login करने के पश्चात्  eMitra plus App पर Go To CRN option पर उपलब्ध CRN Register का चयन करें तथा CRN दर्ज करें। अतः ई-मित्र प्लस मशीन पर आज ही अपनी बायोमेट्रिक उपस्थिति दर्ज करें। - DoIT&amp;C HQ Jaipur. 

</p>

				
				
				
				</div>
<p></p>
<p>

  </p><table class="table table-striped" id="btable">
<thead id="AttendanceDtlsId"></thead>
<tbody id="AttendanceDtlsbody"></tbody>

</table>


<p></p>
				
				<button autofocus="" type="button" class="btn btn-default center-block" data-dismiss="modal">Ok</button>
			</div>

		</div>
	</div>
</div>

<!-- <div class="emitraPlusKioskMsgModal" style="height:187px;width:97%">
	<div class="Close">X</div>
	<div id="messageParagraph" style="overflow: auto;">&#2310;&#2346;&#2325;&#2366; &#2325;&#2368;&#2323;&#2360;&#2381;&#2325; &#2312;-&#2350;&#2367;&#2340;&#2381;&#2352; &#2346;&#2381;&#2354;&#2360; &#2350;&#2358;&#2368;&#2344; &#2360;&#2375; &#2350;&#2376;&#2346; &#2361;&#2376;&#2404; &#2312;-&#2350;&#2367;&#2340;&#2381;&#2352; &#2346;&#2381;&#2354;&#2360; &#2350;&#2358;&#2368;&#2344; &#2346;&#2352; &#2350;&#2376;&#2346; &#2325;&#2367;&#2323;&#2360;&#2381;&#2325; &#2321;&#2346;&#2352;&#2375;&#2335;&#2352; &#2342;&#2381;&#2357;&#2366;&#2352;&#2366; &#2350;&#2366;&#2361; &#2350;&#2375;&#2306; &#2325;&#2350; &#2360;&#2375; &#2325;&#2350; 10 &#2342;&#2367;&#2344; &#2348;&#2366;&#2351;&#2379;&#2350;&#2375;&#2335;&#2381;&#2352;&#2367;&#2325; &#2313;&#2346;&#2360;&#2381;&#2341;&#2367;&#2340;&#2367; &#2342;&#2352;&#2381;&#2332; &#2325;&#2352;&#2344;&#2366; &#2309;&#2344;&#2367;&#2357;&#2366;&#2352;&#2381;&#2351; &#2361;&#2376;&#2404; New eMitra SLA &#2325;&#2375; &#2309;&#2344;&#2369;&#2360;&#2366;&#2352; &#2312;-&#2350;&#2367;&#2340;&#2381;&#2352; &#2346;&#2381;&#2354;&#2360; &#2350;&#2358;&#2368;&#2344; &#2346;&#2352; &#2319;&#2325; &#2350;&#2366;&#2361; &#2350;&#2375;&#2306; 10 &#2342;&#2367;&#2344; &#2360;&#2375; &#2325;&#2350; &#2312;-&#2350;&#2367;&#2340;&#2381;&#2352; &#2346;&#2381;&#2354;&#2360; &#2350;&#2358;&#2368;&#2344; &#2325;&#2367;&#2323;&#2360;&#2381;&#2325; &#2321;&#2346;&#2352;&#2375;&#2335;&#2352; &#2325;&#2368; &#2313;&#2346;&#2360;&#2381;&#2341;&#2367;&#2340;&#2367; &#2346;&#2366;&#2351;&#2375; &#2332;&#2366;&#2344;&#2375; &#2346;&#2352; 500 &#2352;&#2369;&#2346;&#2351;&#2375; &#2325;&#2368; &#2358;&#2366;&#2360;&#2381;&#2340;&#2367; &#2349;&#2368; &#2310;&#2352;&#2379;&#2346;&#2367;&#2340; &#2325;&#2368; &#2332;&#2366;&#2357;&#2375;&#2327;&#2368;&#2404; &#2351;&#2342;&#2367; &#2310;&#2346;&#2325;&#2379; &#2312;-&#2350;&#2367;&#2340;&#2381;&#2352; &#2346;&#2381;&#2354;&#2360; &#2350;&#2358;&#2368;&#2344; &#2346;&#2352; &#2325;&#2368;&#2323;&#2360;&#2381;&#2325; &#2321;&#2346;&#2352;&#2375;&#2335;&#2352; &#2325;&#2368; &#2313;&#2346;&#2360;&#2381;&#2341;&#2367;&#2340;&#2367; &#2342;&#2352;&#2381;&#2332; &#2325;&#2352;&#2344;&#2375; &#2350;&#2375;&#2306; &#2325;&#2379;&#2312; &#2360;&#2350;&#2360;&#2381;&#2351;&#2366; &#2361;&#2376; &#2340;&#2379; &#2360;&#2361;&#2366;&#2351;&#2340;&#2366; &#2361;&#2375;&#2340;&#2369; eMitra Portal &#2346;&#2352; Login &#2325;&#2352;&#2344;&#2375; &#2325;&#2375; &#2346;&#2358;&#2381;&#2330;&#2366;&#2340;&#2381; Home Page &#2346;&#2352; &#2313;&#2346;&#2354;&#2348;&#2381;&#2343;  Register Complaint &#2325;&#2366; &#2330;&#2351;&#2344; &#2325;&#2352;&#2375;&#2306; &#2340;&#2341;&#2366; CRN &#2346;&#2352; &#2313;&#2346;&#2354;&#2348;&#2381;&#2343; &#2357;&#2367;&#2325;&#2354;&#2381;&#2346; &#2350;&#2375;&#2306; Operator Attendance &#2325;&#2366; &#2330;&#2351;&#2344; &#2325;&#2352; &#2342;&#2352;&#2381;&#2332; &#2325;&#2352;&#2375;&#2306;&#2404; 
&#2309;&#2340;&#2307; &#2312;-&#2350;&#2367;&#2340;&#2381;&#2352; &#2346;&#2381;&#2354;&#2360; &#2350;&#2358;&#2368;&#2344; &#2346;&#2352; &#2310;&#2332; &#2361;&#2368; &#2309;&#2346;&#2344;&#2368; &#2348;&#2366;&#2351;&#2379;&#2350;&#2375;&#2335;&#2381;&#2352;&#2367;&#2325; &#2313;&#2346;&#2360;&#2381;&#2341;&#2367;&#2340;&#2367; &#2342;&#2352;&#2381;&#2332; &#2325;&#2352;&#2375;&#2306;&#2404; - DoIT&C HQ Jaipur.</div>
	<div class="bottomMsg">
		<input type="button"
			value="Acknowledge and Close" onclick="acknowledgeEmitraPlusKioskMsg()" />
	</div>
</div> -->

<!-- Bank Account Verification Starts -->

<!-- <div class="modal fade" id="modelBankAccountVerify" role="dialog">
    <div class="modal-dialog" style="width: 80%; background: #fff; padding: 5px;">
    
      Modal content
      <div class="modal-content">
        <div class="modal-header">
          <h4 class="modal-title">Verify your Bank Account</h4>
        </div>
        <div class="modal-body">
          <p>You cannot click outside of this modal to close it.</p>
        </div>
        <div class="modal-footer">
          <button type="button" class="btn btn-default" data-dismiss="modal">Close</button>
        </div>
      </div>
      
    </div>
  </div>
Bank Account Verification Ends

<script>
 $(document).ready(function(){
	$("#modelBankAccountVerify").modal({
		backdrop: "static",
		keyboard:false,
		show:true
	});
}); 
</script> -->
<script src="resources/assets/js/DasboardLinks.js?[B@f2a95a5c"></script>
<script>

function acknowledgeEmitraPlusKioskMsg(){
	$(".emitraPlusKioskMsgModal").fadeOut();
	hideLoadingPopup();
}

$(document).ready(function(){
	if($("#menuList").text().indexOf("Utility") == -1){
		$("#utilLi").hide();
		$("#appLi").hide();
	}

	if($("#menuList").text().indexOf("Application") == -1){
		$("#utilLi").hide();
		$("#appLi").hide();
	}
});

$(document).ready(function(){
//	getQuickPayApps();
	
	
	
		//$('#emitraPlusKioskMsgModal').modal({backdrop: 'static', keyboard: false});
	
	
	$.ajax({
	
		url : 'getKioskBgExpireDate',
		headers : {
			'allow-bypass-header' : 'getKioskBgExpireDate'
		},
		type : 'POST',
		dataType : "json",
		async : false,
		success : function(response) {
		/*console.log(response.vendorBgExpireData);*/
		if(response.vendorBgExpireData.length==0){

			 $('#bgpara').hide();
		}else{
			$.each(response.vendorBgExpireData, function(i, item) {
			
				if(item.isLsp=='Y'){
	
					$('#bgpara').append("<p style='text-align:left;''><span style='color:red'>*Note</span>: <b>Your Lsp BG Expire On</b> <span style='color: red; font-weight: bolder;' >'"+item.expireDate+"'</span><b>, Bg Amount-</b><span style='color: red; font-weight: bolder;'>'"+item.bgAmount+"'</span> <b>, No of days Left - </b><span style='color: red; font-weight: bolder;'>'"+item.noOfDaysRemaining+"'</span></p>");
				}else{		
				
				 $('#bgpara').append("<p style='text-align:left;''><span style='color:red'>*Note</span>: <b>Your BG Expire On</b> <span style='color: red; font-weight: bolder;' >'"+item.expireDate+"'</span><b>, Bg Amount-</b><span style='color: red; font-weight: bolder;'>'"+item.bgAmount+"'</span> <b>, No of days Left - </b><span style='color: red; font-weight: bolder;'>'"+item.noOfDaysRemaining+"'</span></p>");
				} 
				 $('#bgpara').append("<br>")
			});
		}
			
			},
		error : function(data) {
			hideLoadingPopup();
		}
	});

	
	});
	
	function getMyLspCoordinator(){
		showLoadingPopup2();
		$.ajax({
			url : 'getMyLspCoordinatorDetail',
			headers : {
				'allow-bypass-header' : 'getMyLspCoordinatorDetail'
			},
			type : 'POST',
			success : function(data) {
				if(Object.keys(data).length > 0){
					$("#myLspCoordinator").html("");
					$.each(data, function(key, value) {
						$("#myLspCoordinator").append('<div class="form-group col-sm-12">');
						$("#myLspCoordinator").append('<label for="Coorinator Type" class="control-label col-sm-12"><b>Designation: '+value.COORDINATOR_TYPE+'</b></label>');
						$("#myLspCoordinator").append('<label for="Coorinator Name" class="control-label col-sm-12"><b>Name:</b> '+value.NAME+'</label>');
						$("#myLspCoordinator").append('<label for="Coorinator Name" class="control-label col-sm-12"><b>Mobile No.</b>: '+value.MOBILE_NO+'</label>');
						$("#myLspCoordinator").append('<label for="Coorinator Name" class="control-label col-sm-12"><b>Email ID:</b> '+value.EMAIL_ID+'</label>');
						$("#myLspCoordinator").append('</div>');
						$("#myLspCoordinator").append('<hr style="border:1px solid #ececec;margin:0"/>');
							
					});
				}
				hideLoadingPopup2();
			},
			error : function(data) {
				hideLoadingPopup2();
			}
		});
		
	}
	
	function initateCerficatePrinting(vendorCodeValue) {

		$("#certUsrImgCertificate").attr("src",
				"resources/assets/images/default_profile.jpg");
		$("#certHinDistSpan").html("");
		$("#certKioskAdminName").text("");
		$("#certKioskRegAddress").text("");
		$(".certLspNameSpan").text("");
		$("#certKioskCode").text("");
		$("#certKioskPropAddress").text("");
		$(".certKioskNameSpan").text("");
		$("#approvedDate").text("");
		$("#currStatus").text("");
		$("#approverDeptName").text("");

		showLoadingPopup();
		$
				.ajax({
					url : 'getKioskCertificateDetailByVendorCode',
					headers : {
						'allow-bypass-header' : 'getKioskCertificateDetailByVendorCode'
					},
					type : 'POST',
					data : {
						vendorCode : vendorCodeValue
					},
					success : function(data) {
						/*console.log(data);*/

						if (data.PHOTO != undefined && data.PHOTO !="") {
							$("#certUsrImgCertificate").attr("src",
									"data:image/png;base64," + data.PHOTO);
						}

						if (data.DISTRICT_NAME_HIN != undefined) {
							$("#certHinDistSpan").html(
									data.DISTRICT_NAME_HIN);
						}
						if (data.FULL_NAME != undefined) {
							$("#certKioskAdminName").text(data.KIOSK_NAME);
						}
						if (data.REG_ADDRESS != undefined) {
							$("#certKioskRegAddress")
									.text(data.REG_ADDRESS);
						}
						if (data.PARENT_LSP != undefined) {
							$(".certLspNameSpan").text(data.PARENT_LSP);
						}
						if (data.VENDOR_CODE != undefined) {
							$("#certKioskCode").text(data.VENDOR_CODE);
						}
						if (data.PROP_ADDRESS != undefined) {
							$("#certKioskPropAddress").text(
									data.PROP_ADDRESS);
						}
						if (data.KIOSK_NAME != undefined) {
							$(".certKioskNameSpan").text(data.KIOSK_NAME);
						}
						if (data.APPROVED_DATE != undefined) {
							$("#approvedDate").text(data.APPROVED_DATE);
						}
						if (data.CURRENT_STATUS != undefined) {
							if (data.CURRENT_STATUS == "DEFAULTER") {
								$("#currStatus").text("डिफाल्टर");
							} else if (data.CURRENT_STATUS == "BLACKLISTED") {
								$("#currStatus").text("निष्काषित");
							} else if (data.CURRENT_STATUS == "CLOSED") {
								$("#currStatus").text("बन्द");
							} else if (data.CURRENT_STATUS == "ACTIVE") {
								$("#currStatus").text("सक्रिय");
							}else if (data.CURRENT_STATUS == "INACTIVE") {
								$("#currStatus").text("निष्क्रिय");
							}
						}

						$("#approverDeptName")
								.text(data.APPROVER_DEPT_NAME);

						hideLoadingPopup();
						$('#lspKioskCertificatePrinting').modal('show');
					},
					error : function(data) {
						hideLoadingPopup();
					}
				});

	}

	function printKioskCerficate(PrintId) {

		window.innerHTML = "";
		$('.modal-dialog').css({
			'width' : '100%'
		});
		$('.modal-footer').css('display', 'none');
		var mywindow = window
				.open('', 'Print Div', 'height=800,width=1200');
		$(".close").hide();
		$(".printButton").hide();
		mywindow.document.write('<html><head><title></title>');
		mywindow.document.write('</head><body>');
		mywindow.document.write($("#" + PrintId).html());
		mywindow.document.write('</body></html>');

		mywindow.focus(); // necessary for IE >= 10

		mywindow.print();
		mywindow.close();

		$(".close").show();
		$(".printButton").show();
		$('.modal-dialog').css({
			'width' : '80%',
			'padding' : '10px'
		});
		$('.modal-footer').css('display', 'block');

	}

	$('.printButton').click(function() {
		printKioskCerficate('modelCertificatePrint');

	});

//fetchOperatorAttendanceDtls(); 


function fetchOperatorAttendanceDtls(){

	$.ajax({
	
		url : 'fetchOperatorAttendanceDtls',
		headers : {
			'allow-bypass-header' : 'fetchOperatorAttendanceDtls'
		},
		type : 'POST',
		dataType : "json",
		async : false,
		success : function(response) {
/*console.log('dataxx',response);*/
//alert(response.data[0].ADDRESS_DATA);


			var count = 0;

			var entry;
			var name;
			var count;

			entry = response.data[0];
			// alert(entry);
			count = 0;
			var fileHead = "<tr>";
			for (name in entry) {

				fileHead = fileHead + "<th>" + name + "</th>";
				++count;
			}
$('#AttendanceDtlsId').append(fileHead);


$.each(response.data, function( index, value ) {
$('#AttendanceDtlsbody').append('<tr>'); 
$.each(value, function(key, value){
$('#AttendanceDtlsbody').append('<td>'+value+'</td>');  
 });
 $('#AttendanceDtlsbody').append('</tr>'); 

  });
 
 
 




}
});

}

/* var emitraPlusTargetDate = new Date("19-12-2020".replace( /(\d{2})-(\d{2})-(\d{4})/, "$2/$1/$3"));

var todayDate = new Date();
if(todayDate > emitraPlusTargetDate){ 

	$("#tempPlusMsg").hide();
} */




getLink();
function getLink(){
var datax = JSON.parse(dasLinks);
$.each( datax.KioskDasReport, function( key, val ) {
<!-- for DEALING OFFICE BONAFIED -->
let r = Math.random().toString(36).substring(7);
var reportName = val.reportName;
reportName = reportName.toLowerCase();
var reportNameClass = reportName.replace(/[&\/\#,+()$~%. '":*?<>{}]/g, '');

	$('#kioskRep').append('<div class="service-box" id="'+reportNameClass+'" style="width:18%; display:none;"><a class="linktxt" href="'+val.reportUrl+'?'+r+'#"><i class="fa fa-'+val.reportIconClass+' reportBox"></i><p class="text-center reportboxTitle" >'+val.reportName+'</p></a></div>');
	
  });
 
setTimeout(checkContFind, 1000);
}


function checkContFind(){

$('#menuList li a span').each(function(){
var txtmenu = $(this).text();
var txt = txtmenu.replace(/[&\/\#,+()$~%. '":*?<>{}]/g, '');
txt = txt.toLowerCase();
var reportNameClass = txt.replace(/\s/g, '');
/*console.log(reportNameClass);*/

$('#'+reportNameClass).show();

});
}

	
	

</script>
            
									

								</div>
								<!-- END WIDGET TABBED CONTENT -->
								<!-- /content-wrapper -->
							</div>
							<!-- /row -->
						</div>
						<!-- /container -->
						 
					</div>
					<!-- END BOTTOM: LEFT NAV AND RIGHT MAIN CONTENT -->
				</div>
			</div>
	
	
	<!-- END WIDGET TABBED CONTENT -->
	<!-- /content-wrapper -->


	<!-- /row -->
	<!-- /container -->
	<!-- END BOTTOM: LEFT NAV AND RIGHT MAIN CONTENT -->
	<!-- /WRAPPER -->

	<!-- FOOTER -->
	







<script src="resources/assets/js/jquery.min 2.1.4.js"></script>
<script src="resources/assets/js/plugins/datatable/jquery.dataTables-new.min.js"></script>
<script src="resources/assets/js/plugins/datatable/dataTables.bootstrap.min.js"></script>
<script src="resources/assets/js/plugins/datatable/dataTables.buttons.min.js"></script>
<script src="resources/assets/js/plugins/datatable/buttons.bootstrap.min.js"></script>
<script src="resources/assets/js/plugins/datatable/jszip.min.js"></script>
<script src="resources/assets/js/plugins/datatable/plugins/build/pdfmake.min.js"></script>
<script src="resources/assets/js/plugins/datatable/plugins/build/vfs_fonts.js"></script>
<script src="resources/assets/js/plugins/datatable/buttons.html5.min.js"></script>

<script src="resources/assets/js/plugins/datatable/buttons.print.min.js"></script>
<script src="resources/assets/js/plugins/datatable/buttons.colVis.min.js"></script>

<footer class="footer copyYear" style="bottom: 0">© 2023 - 2024<span style="float:right">Build Version V001220720211820 </span></footer>







<!-- Loading popup starts -->
<div class="popup" id="loadingPopUp" style="display: none;">
	<div class="popup-holder" style="width: 100%;">
		<div class="popup-content" style="height: 80px; width: 200px; border-radius: 10px; z-index: 99999">
			<img src="resources/assets/images/preloader.gif"> Please
			Wait...
		</div>
		<!-- popup content -->
	</div>
	<!-- holder -->
</div>
<!-- Loading popup Ends -->


<!-- Loading popup starts -->
<div class="popup" id="loadingPopUp2" style="display: none">
	<div class="popup-holder2">
		<div class="popup-content" style="height: 80px; width: 200px; border-radius: 10px; z-index: 99999">
			<img src="resources/assets/images/preloader.gif"> Please
			Wait...
		</div>
		<!-- popup content -->
	</div>
	<!-- holder -->
</div>
<!-- Loading popup Ends -->

<!-- Common Alert PopUp start -->
<div id="commonAlertPopUpDiv" class="modal fade confirm" role="dialog" style="z-index: 99999999">
	<div class="modal-dialog">

		<!-- Modal content-->
		<div class="modal-content oh" style="border-radius: 8px">
			<div class="modal-body" style="border: 4px solid #EC8239; border-radius: 8px">
				<p>
				</p><div id="commonAlertMessageDiv" class="text-justify"></div>
				<p></p>
				<button autofocus="" type="button" class="btn btn-default center-block" data-dismiss="modal">Ok</button>
			</div>

		</div>
	</div>
</div>
<!-- Common Alert PopUp End -->

<!-- Session Timeout PopUp start -->

<div id="sessionTimeoutPopUpDiv" class="modal fade" role="dialog" style="z-index: 99999">
	<div class="modal-dialog">

		<!-- Modal content-->
		<div class="modal-content preSessionModal">
			<div class="modal-header">
				<h4 class="modal-title">Session is About to Expire!</h4>
			</div>
			<div class="modal-body">
				<div class="text-center msgText">Session will be out in</div>
				<ul class="countdown">
					<li><span class="sessionTime">60</span>
						<p class="seconds_ref">seconds</p></li>
				</ul>

			</div>
			<div class="modal-footer" style="text-align: center">
				<div class="col-sm-12">
					Click
					<button type="button" class="btn btn-default" onclick="dummyAjaxCallToExtendSession()">Extend</button>
					to extend the session!
				</div>
			</div>
		</div>

		<div class="modal-content hide-service postSessionModal">
			<div class="modal-header">
				<h4 class="modal-title">Session is Expired!</h4>
			</div>
			<div class="modal-body">
				<div class="text-center msgText">Your Session is Expired!</div>
			</div>
			<div class="modal-footer" style="text-align: center">
				<div class="col-sm-12">
					<button type="button" class="btn btn-default" onclick="location.reload()">Ok</button>
				</div>
			</div>
		</div>

	</div>
</div>

<style type="text/css">
ul.countdown {
	list-style: none;
	margin: 10px 0;
	padding: 0;
	text-align: center;
}

ul.countdown li span {
	font-size: 80px;
	font-weight: 300;
	line-height: 80px;
}

.msgText {
	font-size: 24px;
	font-style: normal;
}
</style>

<!-- Session Timeout PopUp End -->



<script>
	var currentYear = (new Date).getFullYear();
	varcopyYear = "&copy; " + currentYear + " - " + (currentYear + 1);
	$(".copyYear").html(varcopyYear+'<span style="float:right">Build Version V001220720211820 </span>');
</script>


















<div id="right-box">
	<div class="menu-left-icon" style="right: 0px;">
		<span class="fa fa-chevron-left menu-arrows"></span>
	</div>
	<div class="menu-left-box" style="right: -23%;">		
		<div class="topIcon">
		<div class="center-block text-center">		
		
		
			
			<p><img class="img-avtar" src="resources/assets/images/user-avatar.png" width="100px" alt="User Avatar"></p> 
		
					
			<p><h7> MANOJKUMARBALAI813 </h7></p>
			
			<p><h9>(K12290269)<br>(MANOJ KUMAR BALAI)</h9></p>
			
		</div>
		</div>

		<div class="panel-group" id="accordion">
				


			<div class="panel panel-primary">
				<div class="panel-heading">
					<a class="btn pull-left" data-toggle="collapse" data-parent="#accordion" href="#collapse1"><i class="fa fa-plus"></i></a>
					<h3 class="panel-title">						
						<a data-toggle="collapse" data-parent="#accordion" href="#collapse1">LSP KIOSK</a>
					</h3>
				</div>
				
				
				<div id="collapse1" class="panel-collapse collapse in">				
					<div class="panel-body oh">
						<ul class="list-group" style="overflow-y: auto; max-height:300px;">
						
								<li style="text-indent:0px;cursor: pointer;color:#EC8239" class="list-group-item colorClass" onclick="initiateSwitching('5','5','0')">LSP KIOSK ADMIN</li>
													
						</ul>
					</div>
				</div>
			</div>
			
			


			<div class="panel panel-primary">
				<div class="panel-heading">
					<a class="btn pull-left" data-toggle="collapse" data-parent="#accordion" href="#collapse2"><i class="fa fa-plus"></i></a>
					<h3 class="panel-title">						
						<a data-toggle="collapse" data-parent="#accordion" href="#collapse2">LSP KIOSK OWNER</a>
					</h3>
				</div>
				
				
				<div id="collapse2" class="panel-collapse collapse">				
					<div class="panel-body oh">
						<ul class="list-group" style="overflow-y: auto; max-height:300px;">
						
								<li style="text-indent:0px;cursor: pointer;" class="list-group-item colorClass" onclick="initiateSwitching('9','272','0')">LSP KIOSK OWNER</li>
													
						</ul>
					</div>
				</div>
			</div>
			
			
		
		</div>

	</div>

</div>

<form id="switcherForm" action="switchUserRole" method="post">
	
		<input class="dontDisable" type="hidden" name="switcherLspName" id="switcherLspName" value="CMS COMPUTERS LTD">
	
	<input class="dontDisable" type="hidden" name="ssoId" id="switcherSsoId" value="MANOJKUMARBALAI813">
	<input class="dontDisable" type="hidden" name="tokenNo" id="switcherTokenNo" value="K3BRUXJYRHZNaDBSSmQxQWlaZEVab0FBRFVrOTZRSGx1VE9qVnZPVy9KZ0Z2VXBnWkdqWTBOTjZQSHRMVDAyMDEyQnVRSm9rVkdXV1NCRUd0RjJGa2Vwa0RIa2M2eFlkVkZwN254Y3U1RzJoZnFRVEJxTjFZc2FRelBoUnFER2t1QkRPa1dyOFkveW5Ka1BLZ3owZlNUdE94OVhFbHFURTNDa01ESDU3WXUyRmp5b1Z3NGZLVmVMQ2NpZGFzd2Z3">
	<input class="dontDisable" type="hidden" name="entityTypeId" id="switcherEntityTypeId">
	<input class="dontDisable" type="hidden" name="roleId" id="switcherRoleId">
	<input class="dontDisable" type="hidden" name="officeId" id="switcherOfficeId">
	<input class="dontDisable" type="hidden" name="Role" id="switcherRole" value="5,9">
</form>

<script>

	function initiateSwitching(entityTypeId,roleId,officeId){
		showLoadingPopup();
		if(entityTypeId != "" && roleId != ""){
			$("#switcherEntityTypeId").val(entityTypeId);
			$("#switcherRoleId").val(roleId);
			$("#switcherOfficeId").val(officeId);
			$("#switcherForm").submit();
		}
		
	}

</script>





<!-- <script src="resources/assets/js/jquery.min 2.1.4.js"></script> -->

<script>
	$(".hinLangShow").show();
	$(".engLangShow").hide();
</script>

<script src="resources/assets/js/dist/jquery.validate.js"></script>
<script src="resources/assets/js/validation/commonValidation.js"></script>
<script src="resources/assets/js/table.js"></script>


<script>


	var favActivitiesJs = ["serviceWorkflowForKioskAndCitizen","viewMyInbox"];
	
	
	var reqPage = location.href;
	reqPage = reqPage.substring(reqPage.lastIndexOf("/")+1);
	if(reqPage.indexOf("?") != -1){
		reqPage = reqPage.substring(0,reqPage.lastIndexOf("?"));	
	}
	
	if(favActivitiesJs.indexOf(reqPage) != -1){
		$('#favouriteLink').removeClass("white").addClass("yellow");
	}
	
	var curPath = window.location.href;
	if(curPath.indexOf("?") == -1){
		window.location.hash="``[B@6e2b3f73";//again because google chrome don't insert first hash into history
		window.onhashchange=function(){window.location.hash="[B@7c2ef5d2";}
	}
	else{
		window.location.hash="``";//again because google chrome don't insert first hash into history
		window.onhashchange=function(){window.location.hash="";}
	} 

</script>

<script>
var sessionInterval;
	function sessionTimeOutPopup(counter){
		$('#sessionTimeoutPopUpDiv').modal({backdrop: 'static', keyboard: false},'show');

		sessionInterval = setInterval(function() {
		    counter--;
		    // Display 'counter' wherever you want to display it.
		    if (counter < 0) {
		        // Display a login box
		        clearInterval(sessionInterval);
		        $(".preSessionModal").hide();
		        $(".postSessionModal").show();
		        
		    }
		    else{
		    	$(".sessionTime").text(counter);
		    }
		}, 1000);
	}

	
	function sessionTracker(){
		setTimeout(function() {
			sessionTimeOutPopup(60);
		}, 1740000);	
	}
	sessionTracker();
	
	function dummyAjaxCallToExtendSession() {
		showLoadingPopup();
		$.ajax({
			url : 'dummyAjaxCallToExtendSession',
			headers : {
				'allow-bypass-header' : 'dummyAjaxCallToExtendSession'
			},
			type : 'POST',
			data : {
				extendSession : "Y"
			},
			success : function(data) {
				
				clearInterval(sessionInterval);
				$('#sessionTimeoutPopUpDiv').modal('hide');
				sessionTracker();
				$(".sessionTime").text(60);
				hideLoadingPopup();
			},
			error : function(data) {
				hideLoadingPopup();
			}
		});

	}
	var currentLocation = location.href;
	if(currentLocation.indexOf("editKioskDetailForVerification") == -1 && currentLocation.indexOf("updateCitizenProfile") == -1){
	
		/* $(document).ready(function() {
			$(".popup-holder").css("width", "100%");
			$("#ModalPoliceCharacterPopUpDiv").fadeIn();
		 });*/
	 	
	 $(document).ready(function() {
		showLoadingPopup();
		$.ajax({
			url : 'getCurrentHeaderMarqueeMessage',
			headers : {
				'allow-bypass-header' : 'getCurrentHeaderMarqueeMessage'
			},
			type : 'POST',
			data : {
			},
			success : function(data) {
				if(data !=""){
					$(".headerMarqueeMsg").text($('<div>').html(data).text());
					
				}
				hideLoadingPopup();
			},
			error : function(data) {
				hideLoadingPopup();
			}
		});
	});

	
	}

	$(document).ready(function(){
		  $("#Modal").hide();
		    $(".Ghost-Blue").click(function(){
		      $("#Modal").fadeToggle();
		    });
		    $(".Close").click(function(){
		      $("#Modal").fadeOut();
		    });
		});
</script>



<div class="Modal" id="Modal" style="display: none">
	<!-- <div class="Close">X</div> -->
	<div id="messageParagraph" style="overflow: auto; max-height: 80%"></div>
	<div class="bottomMsg">
		<input type="checkbox" id="iAccept" value="Y"> &nbsp;&nbsp; I have
		read and Acknowledge the message. <input type="button" value="Acknowledge and Close" onclick="acknowledgeMandatoryMsg()">
	</div>
</div>


<div id="ModalPoliceCharacterPopUpDiv" class="ModalPolice" style="z-index: 99999999;display: none">
	<div class="modal-dialog">
		<!-- Modal content-->
		<div class="modal-content oh" style="border-radius: 8px">
			<div class="modal-body" style="border: 4px solid #EC8239; border-radius: 8px">
				<p>
				</p><div id="messageParagraphPoliceCharacterMessageDiv" class="text-justify">प्रिय ई मित्र किओस्कधारक , आपके ई मित्र कीओस्क उपयोगकर्ताओं के पुलिस चरित्र प्रमाण पत्र की वैधता समाप्त हो गयी है / होने वाली है | अत : आप नवीन पुलिस चरित्र प्रमाण पत्र दिनांक 31 मार्च 2023 तक <b>User Management -&gt; Manage User -&gt; Kiosk User Police Verification</b> विकल्प पर जाकर अपलोड करना सुनिश्चित करे |</div>
				<p></p>
				<button autofocus="" type="button" class="btn btn-default center-block" data-dismiss="modal" onclick="acknowledgePoliceCertShowMsg()">Ok</button>
			</div>

		</div>
	</div>
</div>





<script>

	function updateKioskAadharMachineDetail(formid) {
		$("#" + formid).attr("action", "kioskAadharMachineDetailUpdate");
		return true;
	}
	/* Method to Update record for Country End */
	
	/* Method to validate and submit form starts */
	$("#update-kiosk-aadhar-machine-entry").validate({
		 
		submitHandler : function(form) {
			showLoadingPopup();
			$('#btnUpdateAadhar').attr('disabled', true);
			form.submit();
		}
	});
	/* Method to validate and submit form Ends */
	function updateKioskUserMandatoryDetail(formid) {
		$("#" + formid).attr("action", "kioskUserMandatoryFieldSelfUpdate");
		return true;
	}
	/* Method to Update record for Country End */
	
	/* Method to validate and submit form starts */
	$("#update-kiosk-user-required-entry").validate({
		 
		submitHandler : function(form) {
			showLoadingPopup();
			$('#btnUpdate').attr('disabled', true);
			form.submit();
		}
	});
	/* Method to validate and submit form Ends */
	
	/* NESDA work starts */
	function updateKioskUserMandatoryDetail(formid) {
		$("#" + formid).attr("action", "kioskUserNesdaSurveyUpdate");
		return true;
	}
	
	$("#update-nesda-survey-detail-entry").validate({
		 
		submitHandler : function(form) {
			showLoadingPopup();
			$('#btnUpdateNesda').attr('disabled', true);
			form.submit();
		}
	});
	
	/* NESDA work Ends */
	
	$('#disabilityTypeId').unbind("change").change(function() {
		showLoadingPopup();
		getDisabilityDetailList($('#disabilityTypeId').val(), "disabilityDetailId");

	});
	
	$('#deviceName').unbind("change").change(function() {

		if($('#deviceName').val() == "OTHER"){
			$(".otherDeviceNameDiv").slideDown();
		}
		else{
			$(".otherDeviceNameDiv").slideUp();
		}
	});

	
	
	function getDisabilityDetailList(disabilityTypeIdValue, disabilityDetailId) {

		if (disabilityTypeIdValue != "") {
			$.ajax({
				url : 'getDisabilityListByDisabilityType',
				headers : {
					'allow-bypass-header' : 'getDisabilityListByDisabilityType'
				},
				type : 'POST',
				data : {
					disabilityTypeId : disabilityTypeIdValue
				},
				contentType : "application/x-www-form-urlencoded;charset=utf-8",
				success : function(data) {
					/*console.log(data);*/
					var html = '';
					$.each(data, function(key, value) {
						html += '<option value="' + key + '">' + value
								+ '</option>';
					});

					$('#' + disabilityDetailId).html(html);
					autoSortDropdownValues(disabilityDetailId);
					$("#" + disabilityDetailId + " option:selected").prop("selected", false);
					hideLoadingPopup();
				},
				error : function(data) {
					hideLoadingPopup();
				}
			});
		} else {
			var html = '';
			$('#' + disabilityDetailId).html(html);
			hideLoadingPopup();
		}

	}

	$('input:radio[name=disabled]').click(function() {
       if ($(this).attr("value") == "Y") {
           $('#disabilityDiv').show();
         } else{
      	   $('#disabilityDiv').hide();
        }

      });
	
	$('input:radio[name=aadharMachineDeclation]').click(function() {
       if ($(this).attr("value") == "Y") {
           $('#aadharDeviceDetailDataDiv').show();
         } else{
      	   $('#aadharDeviceDetailDataDiv').hide();
        }

      });

	function autoSortDropdownValues(dropDownId) {
		$("#" + dropDownId).html(
				$("#" + dropDownId + " option")
						.sort(
								function(a, b) {
									if (a.value != '' && b.value != '') {
										return a.text.toLowerCase() == b.text
												.toLowerCase() ? 0 : a.text
												.toLowerCase() < b.text
												.toLowerCase() ? -1 : 1;
									}
								}));

		if ($('#' + dropDownId)[0] != undefined) {
			$('#' + dropDownId)[0].selectedIndex = 0;
		}
	}
</script>



<script>
	function acknowledgeMandatoryMsg(){
		if($('input#iAccept').is(':checked')){
			$.ajax({
				url : 'acknowledgeMandatoryMsg',
				headers : {
					'allow-bypass-header' : 'acknowledgeMandatoryMsg'
				},
				type : 'POST',
				data : {
					acknowledge : "Y"
				},
				success : function(data) {
					$("#Modal").fadeOut();
				},
				error : function(data) {
					hideLoadingPopup();
				}
			});
		}
		else{
			showCommonAlertPopup("Please select the I accept Checkbox!");
		}
	}
	
	function acknowledgePoliceCertShowMsg(){
		$.ajax({
			url : 'acknowledgePoliceCertShowMsg',
			headers : {
				'allow-bypass-header' : 'acknowledgePoliceCertShowMsg'
			},
			type : 'POST',
			data : {
				acknowledge : "Y"
			},
			success : function(data) {
				$("#ModalPoliceCharacterPopUpDiv").fadeOut();
			},
			error : function(data) {
				hideLoadingPopup();
			}
		});
	}
	
</script>


<style>
.bottomMsg {
	margin-left: 20px;
}

.Modal,.ModalPolice,.mandatoryFieldModal,.mandatoryAadharDetailModel,.emitraPlusKioskMsgModal,.nesDaSurveyModal {
	height: 100%;
	width: 100%;
	position: fixed;
	top: 0;
	bottom: 0;
	left: 0;
	right: 0;
	margin: auto;
	background: #f1f1f1;
	z-index: 9999;
}


.Modal #messageParagraph,.mandatoryFieldModal #mandatoryFieldData,.mandatoryAadharDetailModel #mandatoryAadharDetailFieldData,.emitraPlusKioskMsgModal,#nesDaSurveyData {
	margin: 20px;
	padding: 10px;
	font-weight: bold;
	font-size: 14px;
	border: 2px solid lightgray;
	border-radius: 5px 5px 5px 5px;
	min-height: 200px;
}

.gov-emitra-logo {
	float: left;
	display: block !important;
	margin: 10px 0 10px 1px !important;
	background: url(http://localhost:8080/emitraApps/resources/assets/images/t-logo.png) no-repeat !important;
	background-size: 160px 58px !important;
	width: 168px;
	height: 52px;
	position: static !important;
	box-shadow: none !important;
}
.avtr-emitra-logo {
	float: right;
	display: block !important;
	margin: 0px 0 0px 0px !important;
	background: url(http://sas-esp-dev:18080/rajSevak/assets/raj.png) no-repeat !important;
	background-size: 66px 69px !important;
	width: 66px;
	height: 69px;
	box-shadow: none !important;
}
div.icon-launch {
	bottom: 20px;
	right: 20px;
	position: absolute;
	height: 95px;
	width: 95px;
	border-radius: 50%;
	cursor: pointer;
	background-size: 100% 100%;
	background-image: url(http://sas-esp-dev:18080/rajSevak/assets/raj.png);
}
</style>

	<!-- END FOOTER -->


	<!-- Javascript -->



	<script src="resources/assets/js/jquery/jquery-2.1.0.min.js"></script>
	<script src="resources/assets/js/bootstrap/bootstrap.min.js"></script>
	<script src="resources/assets/js/plugins/modernizr/modernizr.js"></script>
	<script src="resources/assets/js/plugins/bootstrap-tour/bootstrap-tour.custom.js"></script>
	<script src="resources/assets/js/common.js"></script>
	<script src="resources/assets/js/jquery-ui/jquery-ui-1.10.4.custom.min.js"></script>
	<script src="resources/assets/js/plugins/jquery-slimscroll/jquery.slimscroll.min.js"></script>
	<script src="resources/assets/js/plugins/stat/flot/jquery.flot.min.js"></script>
	<script src="resources/assets/js/plugins/stat/flot/jquery.flot.resize.min.js"></script>
	<script src="resources/assets/js/plugins/stat/flot/jquery.flot.time.min.js"></script>
	<script src="resources/assets/js/plugins/stat/flot/jquery.flot.tooltip.min.js"></script>
	<script src="resources/assets/js/plugins/jquery-sparkline/jquery.sparkline.min.js"></script>
	<script src="resources/assets/js/chart-stat.js"></script>
	<script src="resources/assets/js/plugins/bootstrap-datepicker/bootstrap-datepicker.js"></script>
	<script src="resources/assets/js/plugins/bootstrap-multiselect/bootstrap-multiselect.js"></script>
	<script src="resources/assets/js/jquery.tablesorter.js"></script>

	<script type="text/javascript">
		
	</script>




	<script src="resources/assets/js/plugins/chart/highcharts.js"></script>

	<script src="resources/assets/js/canvasjs.min.js"></script>




	<link href="resources/assets/css/bootstrap-toggle.min.css" rel="stylesheet">
	<script src="resources/assets/js/bootstrap/bootstrap-toggle.min.js"></script>
	<script src="resources/assets/js/DasboardLinks.js"></script>
	
	<div id="popupdivtemp"></div>


	<script type="text/javascript">
	
	
	
		function buildRecentLogChart() {
			if ($("#chartContainersss").val() != null
					&& $("#chartContainersss").val() != undefined) {
				$.ajax({
					url : 'getUserRecentLogDetail',
					headers : {
						'allow-bypass-header' : 'getUserRecentLogDetail'
					},
					type : 'POST',
					success : function(data) {
						//console.log(data);
						$("#dummyPie").remove();
						$("#chartContainersss").show();
						$("#refreshIcon").css({
							'font-size' : '20px',
							'float' : 'right',
							'margin' : '0',
							'position' : 'relative'
						})
						var chart = new CanvasJS.Chart("chartContainersss", {

							title : {
								text : ""
							},
							animationEnabled : true,
							theme : "theme1",
							data : [ {
								type : "doughnut",
								indexLabelFontFamily : "Garamond",
								indexLabelFontSize : 14,
								startAngle : 0,
								indexLabelFontColor : "dimgrey",
								indexLabelLineColor : "darkgrey",
								toolTipContent : "{y} %",

								dataPoints : [

								{
									y : data.SUCESS,
									indexLabel : "SUCCESS {y}%"
								}, {
									y : data.PENDING,
									indexLabel : "PENDING {y}%"
								}, {
									y : data.FAIL,
									indexLabel : "FAIL {y}%"
								},

								]
							} ]
						});

						chart.render();
					},
					error : function(data) {
					}
				});

			}
		}
	</script>



	<script>
		/* Function to fill Favorite Pages Start */
		function loadUserFavPages() {
			$
					.ajax({
						url : 'getUserFavPages',
						headers : {
							'allow-bypass-header' : 'getUserFavPages'
						},
						type : 'POST',
						success : function(data) {
							$("#dragdrop-todo-FP").html("");

							if (Object.keys(data).length > 0) {
								$
										.each(
												data,
												function(key, value) {
													$("#dragdrop-todo-FP")
															.append(
																	'<li><span class="list-control"><span class="handle"><i class="fa fa-bars"></i></span></span><p><strong class="favActivityText">'
																			+ value.activityName
																			+ '</strong><a href="'+value.activityUrl+'" class="favActivity" title="'+value.activityName+'"><span class="label label-danger"  style="top:7px">Open</span></a></p></li>');
												});
							} else {
								$("#dragdrop-todo-FP")
										.append(
												'No Record Found!');
							}
						},
						error : function(data) {
						}
					});
		}
		/* Function to fill Favorite Pages Ends */

		/* Function to fill Favorite Pages Start */
		function loadUserPendingApproval() {
			$
					.ajax({
						url : 'getUserPendingApproval',
						headers : {
							'allow-bypass-header' : 'getUserPendingApproval'
						},
						type : 'POST',
						success : function(data) {
							$("#activityInboxTbody").html("");

							if (Object.keys(data).length > 0) {
								$
										.each(
												data,
												function(key, value) {
													$("#activityInboxTbody")
															.append(
																	'<tr><td>'
																			+ (key + 1)
																			+ '</td><td><input type="hidden" name="regWorkflowLvlId" id="regWorkflowLvlId" value="'+value.regWorkflowLvlId+'"/>'
																			+ value.requestId
																			+ '</td><td>'
																			+ value.entityStr
																			+ '</td><td>'
																			+ value.isGspApplication
																			+ '</td><td>'
																			+ value.isPaypoint
																			+ '</td><td>'
																			+ value.bankBc
																			+ '</td><td>'
																			+ value.isGovtPremises
																			+ '</td><td>'
																			+ value.lspStr
																			+ '</td><td>'
																			+ value.districtStr
																			+ '</td><td>'
																			+ value.oldVendorCode
																			+ '</td><td>'
																			+ value.purpose
																			+ '</td><td>'
																			+ value.regDate
																			+ '</td><td>'
																			+ value.initDate
																			+ '</td><td>'
																			+ value.ssoId
																			+ '</td><td>'
																			+ value.Status
																			+ '</td><td><span class="btn-sm btn-default" style="cursor:pointer;background-color:#1C92AF" onclick="showActivityInboxDetails(\''
																			+ value.vendorProfileId
																			+ '\',\''
																			+ value.entityTypeId
																			+ '\',\''
																			+ value.purpose
																			+ '\',\''
																			+ value.regWorkflowLvlId
																			+ '\')">View</span></td></tr>');
												});
							} else {
								$("#activityInboxTbody")
										.append(
												'<tr><td colspan="7">No Record Found!</td></tr>');
							}
						},
						error : function(data) {
						}
					});
		}
		/* Function to fill Favorite Pages Ends */
		

		



		

		function getQuickPayApps(){
			showLoadingPopup2();
			$.ajax({

				url : 'getQuickPayApps',
				headers : {
					'allow-bypass-header' : 'getQuickPayApps'
				},
				type : 'POST',
				data : {
					},

				success : function(response) {
					
					$("#QuickPay").html("");
					//console.log("response : "+response);
					$.each(response, function(key, value) {
						
						if(value.SRV_ID != '4267' && value.SRV_ID != '4287'){
						$("#QuickPay").append('<div class="service-box" onclick="location.href = \'availService?favSrvId='+value.SRV_ID+'&favSrvName='+value.SRV_NAME+'\'"><i><img src="resources/assets/images/fav.png" class="imgicon"></i><p class="text-center">'+value.SRV_NAME+'</p></div>');
						}
					
						
						
						
						
						
					});
					
					hideLoadingPopup2();
				},
				error : function(xhr, textStatus,
						errorThrown) {
					hideLoadingPopup2();
					console.log('Error in Operation');
				}

			});
		}
		
		/* var win = window.open();
	    win.location = 'https://youtu.be/MEkqExDTMsw';
	    win.opener = null;
	    win.blur();
	    window.focus(); */
		 
		/* webcast URL */
		
		/*  $("#popupdivtemp").append('<form action="//webcast.rajasthan.gov.in/webcast.html" method="get" target="_blank" id="tempPopUpFrmSubmit"></form>');
		$("#tempPopUpFrmSubmit").submit();  */
		
		
	</script>
				
														



</div></div></body>
