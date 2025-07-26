# End-to-End-HR-Dashboard-in-Excel
End-to-End HR Dashboard in Excel – Powered by Oracle DB

## 🔗 Data Source Design

This dashboard uses a dataset that I **created from scratch using Oracle SQL**, which includes:

- `EMPLOYEES` table: ID, Name, Gender, Role, Department, Salary, etc.
- `SCHEDULES` table: Shift timings, break windows
- `ATTRITION` tracking: Resigned/Active flag
- Joined & cleaned using Oracle SQL scripts.

### SQL Sample:

```sql
SELECT department, COUNT(*) AS headcount
FROM employees
WHERE status = 'Active'
GROUP BY department;

so on....
