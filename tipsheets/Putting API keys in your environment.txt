1. Sign up for an API key.
	* Example: you can sign up for a Census API key here: [Census Signup](https://www.google.com/url?sa=t&rct=j&q=&esrc=s&source=web&cd=&cad=rja&uact=8&ved=2ahUKEwi9kv3k0M32AhXLJDQIHbLwC8YQFnoECAYQAQ&url=https%3A%2F%2Fapi.census.gov%2Fdata%2Fkey_signup.html&usg=AOvVaw0hDY_r9WsB_LRLYjcmJsn-)
2. Save your api key somewhere in a text file in a secure place, preferably someplace that is password protected and backed up (I use Dropbox).
3. Download the `usethis` package for R: run `install.packages("usethis")`
4. in the R Console in RStudio, run `usethis::edit_r_environ()`
	* RStudio will open up a new tab called ".Renviron". It will also tell you that you'll have to Restart RStudio for any changes to take effect.
5. In the .Renviron tab, name your key. For example, when using Tidycensus, you want to save your api key as "CENSUS_API_KEY":
	* `CENSUS_API_KEY=xxxxxxx`
	* Replace the xs with your unique API key. No quotes are necessary.
6. Save the .Renviron file, close it, and quit RStudio. Then open it up again. 
7. Your key should be stored in your global environment and ready to use. That means you can use it in any script or project file on your computer. It will only work on your computer, though.