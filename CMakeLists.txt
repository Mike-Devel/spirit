# Copyright 2018 Mike Dev
# Distributed under the Boost Software License, Version 1.0.
# See accompanying file LICENSE_1_0.txt or copy at http://www.boost.org/LICENSE_1_0.txt

cmake_minimum_required(VERSION 3.5)
project(BoostSpirit LANGUAGES CXX)

add_library(boost_spirit INTERFACE)
add_library(Boost::spirit ALIAS boost_spirit)

target_include_directories(boost_spirit INTERFACE include)

target_link_libraries(boost_spirit
    INTERFACE
        Boost::algorithm
        Boost::array
        Boost::assert
        Boost::concept_check
        Boost::config
        Boost::core
        Boost::endian
        Boost::filesystem
        Boost::foreach
        Boost::function
        Boost::function_types
        Boost::fusion
        Boost::integer
        Boost::io
        Boost::iostreams
        Boost::iterator
        Boost::lexical_cast
        Boost::locale
        Boost::math
        Boost::move
        Boost::mpl
        Boost::optional
        Boost::phoenix
        Boost::pool
        Boost::predef
        Boost::preprocessor
        Boost::proto
        Boost::range
        Boost::regex
        Boost::spirit
        Boost::smart_ptr
        Boost::static_assert
        Boost::thread
        Boost::throw_exception
        Boost::tti
        Boost::type_traits
        Boost::typeof
        Boost::unordered
        Boost::utility
        Boost::variant
)
