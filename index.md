## Welcome to GitHub Pages
<script src="https://www.gstatic.com/dialogflow-console/fast/messenger/bootstrap.js?v=1"></script>
<df-messenger
  intent="WELCOME"
  chat-title="prueba"
  agent-id="91b06b9a-21bb-4567-99b6-01828013723e"
  language-code="es"
></df-messenger>
      
         <script>
            // Unsupported fallback:
            var isMobile = (typeof window.orientation !== "undefined") || (navigator.userAgent.indexOf('IEMobile') !== -1);
            var isOpera = (!!window.opr && !!opr.addons) || !!window.opera || navigator.userAgent.indexOf(' OPR/') >= 0;
            var isFirefox = typeof InstallTrigger !== 'undefined';
            var isSafari = /constructor/i.test(window.HTMLElement) || (function (p) { return p.toString() === "[object SafariRemoteNotification]"; })(!window['safari'] || (typeof safari !== 'undefined' && safari.pushNotification));
            var isIE = /*@cc_on!@*/false || !!document.documentMode;
            var isEdge = !isIE && !!window.StyleMedia;
            var isChrome = !!window.chrome; // && (!!window.chrome.webstore || !!window.chrome.runtime);

            var msgContainer = document.getElementById('unsupported-msg');
            // Grab the message DOM right away — if the app loads, it will remove it
            var unsupportedMsg = document.getElementById('unsupported-msg');
            // Once the DOM is ready, proceed
            document.addEventListener('DOMContentLoaded', function(event) {
                // Conditions go here for the necessary requirements
                if (typeof customElements === 'undefined' || isMobile || !(isChrome || isSafari || isFirefox)) {
                    document.getElementsByTagName('html')[0].setAttribute('unsupported', '');
                    // Show our message and add it to the DOM if was removed
                    msgContainer.style.display = 'block';
                    unsupportedMsg.setAttribute('aria-hidden', 'false');
                    document.body.appendChild(unsupportedMsg);
                }
            });
        </script>
        <!-- Feedback API -->
        <script type="text/javascript" src="https://support.google.com/inapp/api.js"></script>
        <!-- Global site tag (gtag.js) - Google Analytics -->
        <script async src="https://www.googletagmanager.com/gtag/js?id=UA-140667198-1"></script>
        <script>
            window.dataLayer = window.dataLayer || [];
            function gtag(){dataLayer.push(arguments);}
            
            function getRedactedPathname(){
                let p = window.location.pathname;
                p = p.replace(/(?<=\/models\/)(\w+)(\/.+)?/gi, "[redacted_id]$2");
                p = p.replace(/(\/train\/\w+\/)(\w+)(\/.+)?/gi, "$1[redacted_drive_id]$3");
                p = p.replace(/(\/drive.+)(\"\w+\")(.+)/gi, "$1[redacted_drive_id]$3")
                p = p.replace(/(\/train.+id=)(\w+)(&.+)/gi, "$1[redacted_drive_id]$3")
                return p;
            }

            gtag('js', new Date());
            gtag('config', 'UA-140667198-1', {
                'custom_map': {
                    'dimension1': 'selected_language'
                },
                'page_path': getRedactedPathname(),
                'referrer' : document.referrer.split('?')[0],
            });            
        </script>
      
You can use the [editor on GitHub](https://github.com/Luiyiee/Luiyiee.github.io/edit/main/index.md) to maintain and preview the content for your website in Markdown files.
