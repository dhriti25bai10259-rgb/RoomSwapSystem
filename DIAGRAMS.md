# Diagram Descriptions

The complete diagram content is included in `REPORT.md` as Mermaid diagrams and text diagrams.

- **Architecture:** User -> RoomSwapSystem -> StudentManager, RoomManager, SwapManager, Admin -> ArrayList collections.
- **Use case:** Student performs student, room, and request actions; Admin views and processes requests.
- **Workflow:** Start -> menu -> operation -> validation -> result -> menu, or exit.
- **Sequence:** Student requests processing; system finds request; Admin chooses an action; SwapManager updates the request and exchanges room values.
- **Class diagram:** RoomSwapSystem connects to managers and Admin; managers own ArrayLists; SwapRequest contains two Student objects.
- **ER diagram:** Not applicable because there is no database; the program uses Java ArrayList collections.
