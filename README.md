# Prisma Fix

[Fix file](prisma/migrations/0_init/migration.sql)

```bash
rm prisma/schema.prisma
rm -rf prisma/migrations/
mkdir prisma/migrations/
mkdir prisma/migrations/0_init/
wget -O prisma/migrations/0_init/migration.sql https://raw.githubusercontent.com/florianamette/toto/refs/heads/main/prisma/migrations/0_init/migration.sql
wget -O prisma/schema.prisma https://raw.githubusercontent.com/florianamette/toto/refs/heads/main/prisma/schema.prisma
npx prisma migrate resolve --applied 0_init
```
 