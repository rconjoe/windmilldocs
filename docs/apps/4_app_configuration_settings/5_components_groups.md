# Group of Components

Components can be grouped within containers. This feature enables making groups generic by having the inner components of it connect to the group fields, therefore building your own meta components.

<video
    className="border-2 rounded-xl object-cover w-full h-full dark:border-gray-800"
    autoPlay
    controls
    id="main-video"
    src="/videos/group_of_components.mp4"
/>

<br/>

Inside those "container groups", you can refer to "group.x" to refer to one of those group field which make this independent of the id of the container itself.

1. From the editor, pick a [container](../4_app_configuration_settings/container.mdx) component and enable "Container is a component group".
2. Create at least one group field.
3. Fill the group field's object, either manually or dynamically through an [eval](../3_app-runnable-panel.mdx#evals).
4. Now the container's components can be [connected](../2_connecting_components/index.mdx) to the group fields items through `group.group_field_name.optional_subitems`

Component groups can be saved to workspace. They will be available from all workspace apps as a component under the "Groups" category.

<video
    className="border-2 rounded-xl object-cover w-full h-full dark:border-gray-800"
    autoPlay
    controls
    src="/videos/save_component_group.mp4"
/>

<br/>

Group of components are saved as resources, under the `app_groups` [folder](../../core_concepts/8_groups_and_folders/index.mdx).