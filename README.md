# SQLPD

## 1. A mailing list of an illegal online service was sent to the SQLPD hot-line. Please submit all entries' details.
```
SELECT * 
FROM mailing_list;
```

## 2. (UMULIT) A mailing list of an illegal online service was sent to the SQLPD hot-line. Please submit all entries' details.
```
SELECT * 
FROM mailing_list;
```

## 3. An illegal site's servers were seized in a recent operation. Please submit all users number of posts and emails' details.
```
SELECT NumberOfPosts, Email 
FROM users;
```

## 4. An illegal site's servers were seized in a recent operation. Please submit all users number of posts, given names and email addresses' details.
```
SELECT NumberOfPosts, GivenName, EmailAddress 
FROM users;
```

## 5. A mailing list of an illegal online service was sent to the SQLPD hot-line. Please submit all records join dates' details. PLease make sure there are no duplicates.
```
SELECT DISTINCT Joined 
FROM mailing_list;
```

## 6. An Illegal site’s servers were seized in a recent operation. Please submit all users' details sorted by last access times in ascending order.
```
SELECT *
FROM users
ORDER BY LastAccess ASC;
```

## 7. An Illegal site’s servers were seized in a recent operation. Please submit all users' details sorted by number of downloads in descending order.
```
SELECT *
FROM users
ORDER BY NumberOfDownloads DESC;
```

## 8. A mailing list of an illegal online service was sent to the SQLPD hot-line. Please submit all entries join dates and surnames' details sorted by surnames in descending order. PLease make sure there are no duplicates.
```
SELECT DISTINCT Joined, Surname
FROM mailing_list
ORDER BY Surname DESC;
```

## 9. A mailing list of an illegal online service was sent to the SQLPD hot-line. Please submit all entries family names, first names, and number of kids' details sorted by family names in ascending order and then by first names in ascending order.
```
SELECT Firstname, FamilyName, NumberOfKids
FROM mailing_list
ORDER BY FamilyName ASC, FirstName ASC;
```

## 10. A mailing list of an illegal online service was sent to the SQLPD hot-line. Please submit the top 10 records' details when sorted by family names in ascending order and then by email addresses in ascending order.
```
SELECT *
FROM mailing_list
ORDER BY FamilyName ASC, EmailAddress ASC
LIMIT 10;
```

## 11. White hat hacker has sent SQLPD exposed subscribers’ details of a shady site connected to various persons of interest. Please submit the top 5 subscribers hashed passwords and subscription dates' details when sorted by hashed passwords in descending order and then by subscription dates in descending order. Please make sure there are no duplicates.
```
SELECT DISTINCT HashedPassword, SubscriptionDate
FROM subscribers
ORDER BY HashPassword DESC, SubscriptionDate DESC
LIMIT 5;
```
