# OmniAuth Manybots

This gem contains the Manybots strategy for OmniAuth.

Manybots uses the OAuth 1.0a flow, you can read about it here: http://www.manybots.com/developers

## How To Use It

Like other OmniAuth 1.0 strategies. If you are using Rails, you need to add this to your `Gemfile`:

	gem "omniauth", ">= 1.0.0"
	gem 'omniauth-manybots', :git => 'https://github.com/NikoRoberts/omniauth-manybots.git'

Then add the following to your `config/initializers/omniauth.rb` (or just the provider line if you have others already):

	Rails.application.config.middleware.use OmniAuth::Builder do
		provider :manybots, "consumer_key", "consumer_secret" 
	end

REMEMBER to replace with your real key and secret, which you get when you register your app with Manybots 

Now just follow the README at: https://github.com/intridea/omniauth

## Supported Rubies

OmniAuth Manybots is tested under 1.9.2

## License

Copyright (c) 2012 by Nicholas Roberts

Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
