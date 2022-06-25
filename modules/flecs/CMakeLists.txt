#-------------------------------------------------------------------------------
#   flecs module
#-------------------------------------------------------------------------------
fips_begin_module(flecs)
    # flecs
    fips_src(flecs/src NO_RECURSE)
    fips_src(flecs/include NO_RECURSE)

    fips_include_directories(flecs/include)

	add_definitions(-D__BAKE__)
    add_definitions(-DUT_IMPL)
fips_end_module()
