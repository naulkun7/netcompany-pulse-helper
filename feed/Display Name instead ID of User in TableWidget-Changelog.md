
```xml
<ComplexType Name="UiMessageSource">

  <Property Name="Action" Type="Edm.String" />

  <Property Name="UserId" Type="Edm.Guid" Nullable="false">

    // Add this line into Feed 

    <Annotation Term="Metadata.IdpUserInfoEnrichment" String="displayName" />

  </Property>

  <Property Name="ActiveRole" Type="Edm.Guid" Nullable="false" />

  <Property Name="Received" Type="Edm.DateTimeOffset" Nullable="false" />

</ComplexType>
```

