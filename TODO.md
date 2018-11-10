# TODO List

## Common
* [Publishing Documentation](https://code.visualstudio.com/docs/extensions/publish-extension#_publishing-extensions)
* Create Marketplace Description
* Add Eyelit Icon for Marketplace

## Highlighting
* [Ideal REGEX Tester as Ruby-based](http://www.rubular.com/)
* [VSCode Documentation](https://code.visualstudio.com/docs/extensionAPI/language-support)
* [TextMate Syntax](https://macromates.com/manual/en/language_grammars)
* [TextMate Tipes & Tricks](https://www.apeth.com/nonblog/stories/textmatebundle.html)
* [Monokai Scope Detector](https://tmtheme-editor.herokuapp.com/#!/editor/local/Monokai)
* Apply Highlighting Rules based on the following REGEX Rules:
  - IF_NULL with all elements as well as () detected IF_NULL Regex:
  (IF_NULL)(\()([^\~]+)\~([^\~\)]+)(\))
- Functions including brackets in separate groups
  \b(TO_NUMBER|TO_INT|TO_DATE|TO_STRING|TO_JSON|JAXB|GET|SET|PUT|ADD|NEW|CONCAT|COALESCE|NESTED_LIST|XPATH|SPLIT_STRING|REPLACE_STRING|TO_NAME_VALUE|PEEK|POP|PUSH|DELAY|DIV|MOD|INCR|CURRENT_POSITION|SIZE|LENGTH|SORT|ADD_ALL)\b(\()(.+)(\))
- Log Function for different coloring
- Functions including brackets in separate groups
  \b(LOG)\b(\()(.+)(\))
- Real multiline Comment REGEX:
  (\/\*([^*]|[\r\n]|(\*+([^*\/]|[\r\n])))*\*+\/)|(\/\/.*)
- Contexts:
  \b(CONTEXT|REQUEST|EVT|REQ|DC|TASK_DC|SPCCHART|TASK_SPC|LOT|OBJ)\b
- RES, RESULT
  \b(RES|RESULT)\b
- /S (color like functions)
  (\/S)
- GOTO Keyword
  \b(goto|GOTO)\b
- Blocks: like Condition:, EXE:, etc.
  ([\w]+\:)
- Loop Controls:
  \b(SCENARIO_LOOP_ELEMENT|SCENARIO_LOOP_CONTROL)\b
- Packages (limit to those making sense!):
  \b(de|com|net|org|java|javax)\b\.+(\w+\.?){1,}
- /P or /TP /ELE
  \b(\/P|\/TP|\/ELE)\b
- Numbers
  [+-]?([0-9]*[.])?[0-9]+
- Comma/Dot/Equal/Tilda
  [\^,.=~]()
- Keywords EMPTY_VECTOR EMPTY_STRING NEWLINE COMMA SPACE null
  \b(EMPTY_VECTOR|EMPTY_STRING|NEWLINE|COMMA|SPACE|null)\b
- MSG.XYZ() or MSG.XYZ(REQ.ABC/P ...)
  \b(MSG)\b(\.)\b(\S+)\b(\()(.*?)(\))
- Special Characters: $
  \$
- Special Characters: =
  \=
- TargetContainer Names
  \b(Action|Action_Category|ActionHub|ActionRequestContainer|ActionRequestTypeContainer|ActionType|Activity|Agent|AR_Status|ArchivePurge|ArchiveRun|Area|Attribute|Basket|Bom|BOMCategory|Calendar|CAP|CAPA|Capa_Category|Capa_Type|Case|CaseList|Cassette|Cassette_Category|CassetteState|CassetteType|Category_Type|ChildConsumableUnit|Condition|Condition_Category|Configuration|Consumable|ConsumableCategory|ConsumableUnit|Context|CPAR_Task|CreateDedicationCode|CreateInhibCode|Criteria|Criteria_Category|Customer|DatabaseColumn|DatabaseTable|DatabaseView|DataSpecification|DecisionHub|DefectCode|DefectCode_Category|Department|Device|Device_Category|Device_Category_Group|DisableDedicationCode|DisableInhibCode|DispatchParameter|DispatchRule|DispatchRuleCategory|DispatchRuleGroup|DocBlobCategory|DocumentBlob|EmploymentStatus|EnableDedicationCode|EnableInhibCode|EncapsulatedEvent|EncapsulatedEventCategory|EncapsulatedEventParameter|EventRedirect|Form|Form_Category|Form_Template|Form_Value|FutureComment|FutureHold|FutureSkipStep|GeneralResourceState|GeneralResourceSubState|Group|HoldCode|ImageMap|ImageMapCategory|Inhibition|Job|JobSchedule|Kpi|KPI_Alert|KPI_Group|LMSRule|Loop|Message|MessageCategory|MfdUnit|MfgStage|MfgStage|MfgStageCategory|ObjectType|Operation|Operation_Category|OperationType|Printer|Product|Product_Category|ProductType|Profile|QPAR_Status|Query|QueryCategory|RDA|Recipe|RecipeCategory|RecipeParameter|RecipeTemplate|RecipeTemplateCategory|ReleaseCode|Report|ReportCategory|Request|Reservation|ResolutionCode|ResolutionCode_Category|Resource_Capability|ResourcePriority|ResourceState|ResourceSubState|Reticle|Reticle_Category|ReticlePod|ReticlePodCategory|ReworkCode|RunValue|SamplingPlan|Scenario|ScenarioCategory|ScrapCode|Shift|SignatureHub|SignatureState|Site|SparePart|SparePartCategory|SPC|SPCAnnotation|SPCCategory|SPCFilter|SplitCode|Step|Step_Category|SubArea|Subject|SubRecipe|SubRecipeCategory|Supplier|SupplierCategory|SWR|SWRSetLotStructDef|SWRStepStructure|Task|TaskOperation|ToolAlarm|ToolAlarmCategory|ToolRelation|ToolRunDataset|ToolTransition|Training_Category|TrainingDocument|TrainingDocumentState|TrainingReviewSchedule|TrainingSchedule|TrainingState|Transaction|TransService|UIEvent|UIEventCategory|UIFilter|UISorter|UITableDescriptor|UnscrapCode|User|User_Category|UserEmploymentStatus|UserSection|UserShift|ValueSpec|Variable|WIPCategory|WIPState|WIPType|Workflow|Workflow_Category|WorkOrder|WorkOrderCategory|WorkOrderElement)/b

## Snippets
* [VSCode Documentation](https://code.visualstudio.com/docs/editor/userdefinedsnippets)
* Add DOM Handling
* Add common views (multi-line; common parameters, common RES access)
  * com.eyelit.ads.importer.view.ADSPerformMfdUnitScrapView
  * com.eyelit.ads.importer.view.ADSPerformModifyAttributesView
  * com.eyelit.ads.importer.view.ADSPerformModifyTaskAttributesView
  * com.eyelit.ads.importer.view.ADSPerformModifyVariablesView
  * com.eyelit.view.AddMfdUnitHoldView
  * com.eyelit.view.AttributeReferencesView
  * com.eyelit.view.AutomationCreateAndPerformReworkView
  * com.eyelit.view.AutomationCreateObjectAssociationView
  * com.eyelit.view.AutomationPerformLoadResourceOperationView
  * com.eyelit.view.AutomationPerformMaterialConsumptionView
  * com.eyelit.view.AutomationPerformNextView
  * com.eyelit.view.AutomationStartLotView
  * com.eyelit.view.ChangeActiveFlagView
  * com.eyelit.view.ChangeMfdUnitProductView
  * com.eyelit.view.ChangeMfdUnitStateView
  * com.eyelit.view.ChangeResourceStatusView
  * com.eyelit.view.ConsumableUnitComponentsView
  * com.eyelit.view.ConsumableUnitHeaderView
  * com.eyelit.view.ContainerReferencesView
  * com.eyelit.view.CreateInhibitionThroughConditionView
  * com.eyelit.view.DefaultObjectUpdateView
  * com.eyelit.view.DisplayMsgView
  * com.eyelit.view.HoldTaskSAView
  * com.eyelit.view.MfdUnitContentView
  * com.eyelit.view.ObjectAttributesView
  * com.eyelit.view.ObjectDetailsView
  * com.eyelit.view.PerformMfdUnitAdHocRepositionView
  * com.eyelit.view.RetrieveObjectByAliasView
  * com.eyelit.view.RetrieveObjectsByPropertyView
  * com.eyelit.view.RetrieveObjectView
  * com.eyelit.view.ScenarioExecutionView
  * com.eyelit.view.ScheduleTaskView
  * com.eyelit.view.SendMailView
  * com.eyelit.view.SimpleDatabaseRequest
  * com.eyelit.view.UpdateExtendedMfdUnitView
  * com.eyelit.view.UpdateGeneralResourceStatusView
  * com.eyelit.view.UpdateObjectAttributesView
  * com.eyelit.view.UpdateObjectVariablesView
  * com.eyelit.view.UpdateResourceCommentView
  * com.eyelit.view.UpdateUnitInfoView
  * com.eyelit.view.VariableResolveView
* Add typical context elements (see Eyelit Scenario Guide)
* Add list of commonly used attributes
* Add list of commonly used variables
