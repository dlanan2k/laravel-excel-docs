# Export concerns

| Interface | Explanation |
|---- |----|
|`Maatwebsite\Excel\Concerns\FromCollection`| Use a Laravel Collection to populate the export. |
|`Maatwebsite\Excel\Concerns\FromQuery`| Use an Eloquent query to populate the export. | 
|`Maatwebsite\Excel\Concerns\FromView`| Use a (Blade) view to to populate the export. |
|`Maatwebsite\Excel\Concerns\WithTitle`| Set the Workbook or Worksheet title. |
|`Maatwebsite\Excel\Concerns\WithHeadings`| Prepend a heading row. |
|`Maatwebsite\Excel\Concerns\WithMapping`| Format the row before it's written to the file. |
|`Maatwebsite\Excel\Concerns\WithColumnFormatting`| Format certain columns. |
|`Maatwebsite\Excel\Concerns\WithMultipleSheets`| Enable multi-sheet support. Each sheet can have its own concerns (except this one). |
|`Maatwebsite\Excel\Concerns\ShouldAutoSize`| Auto-size the columns in the worksheet. |
|`Maatwebsite\Excel\Concerns\WithStrictNullComparison`| Uses strict comparisions when testing cells for null value. |
|`Maatwebsite\Excel\Concerns\WithEvents`| Register events to hook into the PhpSpreadsheet process. |
|`Maatwebsite\Excel\Concerns\WithCustomQuerySize`| Allows Exportables that implement the FromQuery concern, to provide their own custom query size. |
|`Maatwebsite\Excel\Concerns\WithCustomCsvSettings`| Allows to run custom Csv settings for this specific exportable. |
|`Maatwebsite\Excel\Concerns\WithCharts`| Allows to run one or multiple PhpSpreadsheet Chart instances. |
|`Maatwebsite\Excel\Concerns\WithDrawings`| Allows to run one or multiple PhpSpreadsheet (Base)Drawing instances. |
|`Maatwebsite\Excel\Concerns\WithCustomStartCell`| Allows to specify a custom start cell. Do note that this is only supported for FromCollection exports. |

### Traits

| Trait | Explanation |
|---- |----|
|`Maatwebsite\Excel\Concerns\Exportable` | Add download/store abilities right on the export class itself.
|`Maatwebsite\Excel\Concerns\RegistersEventListeners` | Auto-register the available event listeners. | 
