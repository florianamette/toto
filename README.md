# Prisma Fix

[Fix file](prisma/migrations/0_init/migration.sql)

```bash
mkdir prisma/migrations/0_init
rm prisma/schema.prisma
wget -O prisma/migrations/0_init/migration.sql https://raw.githubusercontent.com/prisma/prisma-examples/latest/typescript/rest-nextjs-prisma-mysql/prisma/migrations/0_init/migration.sql
npx prisma migrate resolve --applied 0_init
```
 