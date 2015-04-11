# node-soap-servicegenerator

This generator will generate a lot of useful code, but it's still a work in progress.

I created this generator to generate node-soap service stubs from the Onvif.org wsdl's so I don't have to look everything up all the time :)
It is far from perfect and still requires you to look up, for example, enum types, but it generates a lot of usefull code anyway.

I plan on improving and perfecting this, but first I want to spend some time on the project I created this generator for :)

You can use it by running it from your IDE and just edit the options:

	var options = {
	  wsdl : "./test-wsdl/media_service.wsdl",
	  output : "./test-output/media_service.js",
	  ignoredTypes : "[NetworkZeroConfigurationExtension,Transport]",
	  tab : "  ",
	  lineEnd : "\n",
	  maxdepth : "25",
	  throwFaults : "true"
	};

Or just run "node generate.js option=value option=value option=value etc.."
Just note that the strings in the array do not require a quote:"
