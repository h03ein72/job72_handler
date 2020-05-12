# Job72 Handler
This is a simple FiveM-Script for those whom need a limiter for jobs.

## Requirements
- Ghmattimysql | [GitHub](https://github.com/GHMatti/ghmattimysql)
- Essentialmode | [GitHub](https://github.com/kanersps/essentialmode)
- ES-Extended | [GitHub](https://github.com/ESX-Org/es_extended)

## Installation
Just use this to set a checker

```
ESX.TriggerServerCallback('job72_handler:getTimers', function(isExpired)

    if isExpired then

        ESX.ShowNotification("~y~You are ~r~Finished. ~y~Call admin to recharge.")

    else
        
        -- your code

    end

end, ESX.PlayerData.job.name)
```

Then use these commands to set or delete the timers:
    /rtjob
    /rdjob
