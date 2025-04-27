<html>
<body>
  Hello
  <script type='text/javascript'>
	function initEmbeddedMessaging() {
		try {
			embeddedservice_bootstrap.settings.language = 'en_US'; // For example, enter 'en' or 'en-US'

			embeddedservice_bootstrap.init(
				'00DHr00000Df2UV',
				'GithubKiru',
				'https://ecloudsagentforce.my.site.com/ESWGithubKiru1745723634825',
				{
					scrt2URL: 'https://ecloudsagentforce.my.salesforce-scrt.com'
				}
			);
		} catch (err) {
			console.error('Error loading Embedded Messaging: ', err);
		}
	};
</script>
<script type='text/javascript' src='https://ecloudsagentforce.my.site.com/ESWGithubKiru1745723634825/assets/js/bootstrap.min.js' onload='initEmbeddedMessaging()'></script>

</body>
  
</html>
