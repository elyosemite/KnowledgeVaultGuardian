# Entity Framework

Entity Framework supports ``Enum`` in your model.

We define `Department.cs`:
```csharp
public enum DepartmentNames
{
    English,
    Math,
    Economics
}     

public partial class Department
{
    public int DepartmentID { get; set; }
    public DepartmentNames Name { get; set; }
    public decimal Budget { get; set; }
}
```

in `Program.cs`

```csharp
using System.Data.Entity;

public partial class EnumTestContext : DbContext
{
    public DbSet<Department> Departments { get; set; }
}

using (var context = new EnumTestContext())
{
    context.Departments.Add(new Department { Name = DepartmentNames.English });

    context.SaveChanges();

    var department = (from d in context.Departments
                        where d.Name == DepartmentNames.English
                        select d).FirstOrDefault();

    Console.WriteLine(
        "DepartmentID: {0} Name: {1}",
        department.DepartmentID,  
        department.Name);
}
```

The output is:

```bash
DepartmentID: 1 Name: English
```

# Link
- https://learn.microsoft.com/en-us/ef/ef6/modeling/code-first/data-types/enums