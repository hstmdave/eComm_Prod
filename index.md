<script type='text/javascript'>
	function initEmbeddedMessaging() {
		try {
			embeddedservice_bootstrap.settings.language = 'en_US'; // For example, enter 'en' or 'en-US'

      window.addEventListener("onEmbeddedMessagingReady", () => {
            			embeddedservice_bootstrap.prechatAPI.setHiddenPrechatFields({
                			"PreChat_URL": window.location.origin
            			});
        		});
      
			embeddedservice_bootstrap.init(
				'00D300000006Vym',
				'Messaging_eCommerce',
				'https://healthstream.my.site.com/ESWMessagingeCommerce1763566012249',
				{
					scrt2URL: 'https://healthstream.my.salesforce-scrt.com'
				}
			);
		} catch (err) {
			console.error('Error loading Embedded Messaging: ', err);
		}
	};
</script>
<script type='text/javascript' src='https://healthstream.my.site.com/ESWMessagingeCommerce1763566012249/assets/js/bootstrap.min.js' onload='initEmbeddedMessaging()'></script>
