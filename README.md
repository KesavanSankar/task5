# task5

For determining which users can be labeled as adopted users,
we can use groupby and rolling methods to find the users who were active for more than 3 days in any of the 7 day rolling period.

If any of the values in the visits_7_days column is >=3, then we can label that user as adopted.

The null values in the adopted_user and last_session_creation_time can be filled in with 0 because we can assume that those users aren't adopted users.
There are too many email domains and most of them seem fake domains so it's good to drop the column entirely. We can also drop the name and object_id columns.

