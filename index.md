<html>
    <body>
        <script type="text/javascript">
            function initEmbeddedMessaging() {
                try {
                    embeddedservice_bootstrap.settings.language = "en";

                    window.addEventListener("onEmbeddedMessagingReady", () => {            
                        console.log( "Inside Prechat API!!" );
                        embeddedservice_bootstrap.prechatAPI.setHiddenPrechatFields( { "Order_Number" : "Test123" } );
                    });

                    embeddedservice_bootstrap.init( "00D8Z000000sp44", "Messaging_for_In_App_and_Web_GitHub_with_Omni_Flow", "https://infallibletechiemiaw.my.site.com/ESWMessagingforInAppa1676401841646", {
                        scrt2URL: "https://infallibletechiemiaw.my.salesforce-scrt.com",
                    } );
                } catch ( err ) {
                    console.error( "Error loading Embedded Messaging: ", err );
                }
            }
        </script>
        <script type="text/javascript" src="https://infallibletechiemiaw.my.site.com/ESWMessagingforInAppa1676401841646/assets/js/bootstrap.min.js" onload="initEmbeddedMessaging()"></script>
    </body>
</html>
