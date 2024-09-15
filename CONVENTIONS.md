# FASTAPI CONVENTIONS

- Excessively use Pydantic
- Serializes all datetime fields to a standard format with an explicit timezone
- Decouple & Reuse dependencies in your API code. Dependency calls are cached.
- Use dependencies for data validation vs DB
- Don’t make your routes async, if you have only blocking I/O operations
- Migrations. Alembic
- Background Tasks > asyncio.create_task
- Be careful with dynamic pydantic fields
- Save files in chunks
  If you must use sync SDK, then run it in a thread pool.
