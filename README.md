### For cmprovider Sakai 10 patch

- Copy cmprovider from Sakai 11 into the top level of your Sakai 10 source
- Apply cmprovider_sakai10.patch
- Run the following SQL statement to add the dropDate field to enrollments

```sql
ALTER TABLE CM_ENROLLMENT_T ADD COLUMN DROP_DATE DATE;
```
