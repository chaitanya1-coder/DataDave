In this project, I integrated the New Relic APM (Application Performance Monitoring) agent into a Python-based game application called Data Dave. The primary goal was to monitor application performance, gather detailed insights into system metrics, and improve the overall efficiency of the game.

### New Relic is a cloud-based platform that provides real-time insights into the performance and behavior of digital systems.
With the help of New Relic we can do, Application performance monitoring (APM), Infrastructure monitoring, Log management, Vulnerability management and so on.

New Relic Account ID- 4726082, 
Email address used for creating the New Relic Account- chaitanyajobwork@gmail.com

## Running the program

- You can run the game by running the main python script located at the root of the repository: `NEW_RELIC_CONFIG_FILE=newrelic.ini newrelic-admin run-program python game.py`. This should start the game immediately.

---

## Primary Goals for this project :

1. New Relic instrumentation

- Set up instrumentation for the application.

- Update the newrelic.ini file by replacing INSERT_YOUR_INGEST_LICENSE_KEY_HERE with your account's [ingest license key](https://docs.newrelic.com/docs/apis/intro-apis/new-relic-api-keys/).

2. Setup Custom Dashboard

  - To see your game stats on a New Relic dashboard edit the [game_stats.json](game_stats.json) file by doing a global search and replace to substitute "YOUR_ACCOUNT_ID" with your 7-digit [account ID](https://docs.newrelic.com/docs/accounts/accounts-billing/account-structure/account-id/).

  - Then, copy the modified JSON and [import the dashboard](https://docs.newrelic.com/docs/query-your-data/explore-query-data/dashboards/introduction-dashboards/#dashboards-import) into your New Relic account.
    
3. Custom Instrumentation
  - Evaluate the [game_stats.json](game_stats.json) and setup custom instrumentation for all the custom events similar to the example provided in the `game.py`.
  - Try to capture **MOST** of the events if not all
  - Refer to the sample of the [populated dashboard](Game_Stats-Dashboard_sample.pdf) (file:Game_Stats-Dashboard_sample.pdf) included in the zip folder

---

## Troubleshooting

- If the game is crashing or you are unable to run the game, make sure you have complete the prerequisites above especially the ENV VAR and adding New Relic License Key to the `newrelic.ini` file.
- After adding the ENV VAR (`export NEW_RELIC_CONFIG_FILE=/Users/username/Downloads/dangerous-dave/newrelic.ini`), launch the game using the binary from the same terminal instance. Alternatively you can add the ENV VAR to your `.bashrc`, `.zshrc` or `.bash_profile` file and restart your terminal session.

---

### Dangerous Dave Replica
*(this is the original description you can find over on https://github.com/mwolfart/dangerous-dave) We remain deeply indebted to them for their effort to bring this classic game to life on the python platform! - Rachel and Leon)*

 - This project is a replica of the 1988 DOS game Dangerous Dave, made by John Romero. The project was built in Python along with a team of three students (Arthur Medeiros, Guilherme Cattani and me), as a course assignment.
 - The goal of the project was to study and practice the three types of programming paradigms: imperative, object-oriented and functional. To achieve this, we picked Python as a language since it can perform all three types of tasks in a fairly good way.


