on run
	
	set currentDay to weekday of (get current date)
	
	if currentDay is in {Monday, Tuesday, Wednesday, Thursday} then
		
		set akt_time to (time of (current date))
		# set actual time to akt_time
		set feierabend_mo_do to "60600"
		# In this example the end time is 4:50 PM (H*M*S)+(M*S) (16*60*60)+(50*60)=60.600 seconds
		
		set diff_time to (feierabend_mo_do - akt_time)
		set diff_time_minutes to (round (diff_time / 60))
		
		
		if diff_time_minutes > 0 then
			tell application "Amphetamine" to start new session with options {duration:diff_time_minutes, interval:minutes, displaySleepAllowed:false}
		else
			log diff_time_minutes
		end if
		
	end if
	
	if currentDay is in {Friday} then
		
		set akt_time to (time of (current date))
		set feierabend_fr to "46200"
		
		set diff_time to (feierabend_fr - akt_time)
		set diff_time_minutes to (round (diff_time / 60))
		
		
		if diff_time_minutes > 0 then
			tell application "Amphetamine" to start new session with options {duration:diff_time_minutes, interval:minutes, displaySleepAllowed:false}
		else
			log diff_time_minutes
		end if
		
	end if
end run
