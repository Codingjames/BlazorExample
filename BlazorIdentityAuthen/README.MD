#How to ?
- 1. Create Blazor Wasm choose "Hosted" And "Individual"
- 2. Change Config aim to target SqlServer in Setting.cs
- 3. Add migration and update database 

```
	- Dotnet CLI
	dotnet ef migrations add migration_name [-c ContextName]
	dotnet ef database update [-c ContextName]

	- Package Manager
	add-Migration migration_name [-Context ContextName]
	update-database [-Context ContextName]
```

4 Add Identity scaffold 
5 remove duplicate context in Property.cs
6 Try run.