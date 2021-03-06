If you copy a database between environments, the copied database won't be fully functional until you run the Environment reprovisioning tool to make sure that all Retail components are up to date.

> [!IMPORTANT]
> We recommend that you complete this procedure even if you don't use Retail components, because Retail functionality is included in all environments. 

Before you continue, you must make sure that the following prerequisites are met:

1. The appropriate updates are applied to the target environment:

    - If the target environment runs the 7.3 release (December 2017), apply this update:

        - KB 4091254

    - If the target environment runs the July 2017 release (7.2), apply these updates:

        - KB 4035399
        - KB 4045801
        - KB 4091255

    - If the target environment runs version 1611 (November 2016, the 7.1 release), apply these updates:

        - KB 4025631
        - KB 4035355
        - KB 4035492
        - KB 4010947

2. Both the default channel database and the default channel data group must be named **Default**. If you've renamed them, you must change the names back.

Follow these steps to run the Environment reprovisioning tool.

1. In your project's **Asset Library**, in the **Software deployable packages** section, click **Import**.
2. From the list of shared assets, select the **Environment Reprovisioning Tool**.
3. On the **Environment details** page for your target environment, select **Maintain** > **Apply updates**.
4. Select the **Environment Reprovisioning** tool that you uploaded earlier, and then select **Apply** to apply the package.
5. Monitor the progress of the package deployment. 

For more information about how to apply a deployable package, see [Apply a deployable package](../deployment/create-apply-deployable-package.md). For more information about how to manually apply a deployable package, see [Install a deployable package](../deployment/install-deployable-package.md).
